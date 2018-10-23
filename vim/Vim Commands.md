# Vim Commands

## help

The most import thing to learn about in vim is...

```markdown
:help
```

and

```
:help command
```

- TAB - cycles through possible command completions

- CTRL-d - lists possible command completions

  For example, try

```
:help tags (then CTRL-d and TAB)
```

- Do **help i_ CTRL-d** for insert commands, **v_** for visual, etc.
- Also, when in the help pages, **CTRL-]** jumps to subjects between |bars| and **CTRL-T** jumps back (and, of course, :q to quit).

## Additional Command

```
dd/yy => delete/yank the current line
D/C => delete/change until the end of line
^/$ => move to the beginning/end of line
I/A => move to the beginning/end of line and insert
o/O => insert new line below/above current line and insert
```

## Abreviations

```
a => all
i => inside
t => untill
f => forward
```

## Delete

```markdown
d d => deletes the current line
d i w => delete in word (deletes the whole word under cursor)
c a w => change all word (deletes the whole word under cursor and puts in insert mode)
d i ) => yank all text inside parentheses (deletes all the words inside the parentheses)
d a ) => deletes all inside parentheses inclduing parentheses
d t space => deletes untill the space
d f space => deletes with the space
```

## Copy and Paste

```
y y => copies the current line
p => paste below the line
P => paste above the line
<C-r>{register} => paste in Instert Mode
```

##Select

```markdown
v a " => visually selects all inside doublequotes including doublequotes
```

## Repeatition

```
. => repeats the last command
```

## Record a Macro

- Recording :- 

  ```
  q{register}
  (do the things)
  q
  ```


- Playing a Macro :-

  ```
  @{register}
  ```

## Tmux

- Tmux session creating :-

  ```
  tmux new-session -s {session-name}
  ```


## Reformatting

- These are useful to reformat text paragraphs or chunks of code (NOTE: this does *not* work for python code...):

```
V=  => select text, then reformat with =
=   => will correct alignment of code
==  => one line; 
gq  => reformat paragraph
```

- Options to change how automatic formatting is done:

```
    :set formatoptions (default "tcq")
        t - textwidth
        c - comments (plus leader -- see :help comments)
        q - allogw 'gq' to work
        n - numbered lists
        2 - keep second line indent
        1 - single letter words on next line
        r - (in mail) comment leader after 
```

- Other related options:

```
    :set wrapmargin
    :set textwidth
```

## Word & line completion

- Typing is a pain! In *insert* mode, try:

```
ctrl-n, ctrl-p    - next/previous word completion 
                    (similar word in current file)

ctrl-x ctrl-l (ctrl-n/p)    - line completion

:set dictionary=/usr/share/dict/words
ctrl-x ctrl-k     - dictionary completion
```

- also

```
ctrl-w      - erases word (insert mode...
ctrl-u      - erases line  ...or on command line)
```

## Searching

- For basic searching:

```
/pattern       - search forward for pattern
?pattern       - search backward
n              - repeat forward search
N              - repeat backward
```

- Some variables you might want to set:

```
:set ignorecase - case insensitive
:set smartcase  - use case if any caps used 
:set incsearch  - show match as search proceeds
:set hlsearch   - search highlighting
```

More cool searching tricks:

```
*               - search for word currently under cursor
g*              - search for partial word under cursor 
                  (repeat with n)
ctrl-o, ctrl-i  - go through jump locations
[I              - show lines with matching word under cursor
```

Search and replace...

```
:%s/search_for_this/replace_with_this/    - search whole file and replace
:%s/search_for_this/replace_with_this/c   - confirm each replace
```
## Text selection

- If you want to do the same thing to a collection of lines, like cut, copy, sort, or format, you first need to select the text. Get out of insert mode, hit one of the options below, and then move up or down a few lines. You should see the selected text highlighted.

```
V       - selects entire lines 
v       - selects range of text
ctrl-v  - selects columns
gv      - reselect block
```

- After selecting the text, try d to delete, or y to copy, or :s/match/replace/, or :center, or !sort, or...
- Here's one way to move selected text over a few spaces:

```
 - select a chunk of code using capital V and the arrow keys (or j, k)
 - type colon
 - then type s/^/   /
 - hit return
```

- What you've done is replace the beginning of each selected line (the ^ symbol means "the beginning of the line") with spaces.

## Repeatable Actions and How to Reverse them

| Intent                           | Act                  | Repeat | Reverse |
| -------------------------------- | -------------------- | :----- | :------ |
| Make a change                    | {edit}               | .      | u       |
| Scan line for next character     | f{char}/t{char}      | ;      | ,       |
| Scan line for previous character | F{char}/T{char}      | ;      | ,       |
| Scan document for next match     | /pattern<CR>         | n      | N       |
| Scan document for previous match | ?pattern<CR>         | n      | N       |
| Perform substitution             | :s/target/replacemnt | &      | u       |
| Execute a sequence of changes    | qx{changes}q         | @x     | u       |

## Vim's Operators Commands

| Trigger | Effect                                                  |
| ------- | ------------------------------------------------------- |
| c       | Change                                                  |
| d       | Delete                                                  |
| y       | Yank into a register                                    |
| g~      | Swap Case                                               |
| gu      | Make Lowercase                                          |
| gU      | Make Uppercase                                          |
| >       | Shift Right                                             |
| <       | Shift Left                                              |
| =       | Autoindent                                              |
| !       | Filter {motion} lines <br />through an external program |

## Keystrokes for deleting in Insert Mode

| Keystrokes   | Effect                                |
| ------------ | ------------------------------------- |
| **Ctrl + h** | Delete back one character {Backspace} |
| **Ctrl + w** | Delete back one word                  |
| **Ctrl + u** | Delete back to start of line          |

## Paste in Instert Mode

The **Ctrl + r{register}** command is convenient for pasting a few words from Insert
mode. If the register contains a lot of text, you might notice a slight delay
before the screen updates. That’s because Vim inserts the text from the reg-
ister as if it were being typed one character at a time. If the ‘textwidth’ or
‘autoindent’ options are enabled, you might end up with unwanted line breaks
or extra indentation.
The **Ctrl + r + Ctrl + p{register}** command is smarter. It inserts text literally and fixes
any unintended indentation (see :h i_CTRL-R_CTRL-P ). But it’s a bit of a handful!
If I want to paste a register containing multiple lines of text, I prefer to switch
to Normal mode and use one of the put commands

## Expression Register

- **<Ctrl + r>=** 
- This opens a prompt at the bottom of the screen
  where we can type the expression that we want to evaluate. When done, we
  hit **Enter** , and Vim inserts the result at our current position in the document.

## Visual Mode 

| Command      | Effect                              |
| ------------ | ----------------------------------- |
| v            | Enable character-wise visual mode   |
| V            | Enable line-wise visual mode        |
| **Ctrl + v** | Enable block-wise visual mode       |
| gv           | Reselect the  last visual selection |

## Command Mode

| Command                                        | Effect                                                       |
| ---------------------------------------------- | ------------------------------------------------------------ |
| :[range]delete [x]                             | Delete specified lines [into register x]<br/>                |
| :[range]yank [x]                               | Yank specified lines [into register x]                       |
| :[line]put [x]                                 | Put the text from register x after the specified line        |
| :[range]copy {address}                         | Copy the specified lines to below the line specified<br/>by {address} |
| :[range]move {address}                         | Move the specified lines to below the line specified<br/>by {address} |
| :[range]join                                   | Join the specified lines                                     |
| **:[range]normal {commands}**                  | Execute Normal mode {commands} on each speci-<br/>fied line  |
| :[range]substitute/{pat-tern}/{string}/[flags] | Replace occurrences of {pattern} with {string} on each specified line |
| :[range]global/{pattern}/[cmd]                 | Execute the Ex command [cmd] on all specified<br/>lines where the {pattern} matches |
| :[range]move {address} / :[range]m {address}   | Move lines                                                   |
| :[range]copy {address} / :[range]t {address}   | Copy lines                                                   |
| @:                                             | **Repeats the last Ex Command**<br />After running **@:** for the first time, we can subsequently repeat it with the **@@** command. |
| q/                                             | Open the command-line window with history of searches        |
| q:                                             | Open the command-line window with history of Ex commands     |
| **Ctrl + f**                                   | Switch from Command-Line mode to the command-line window     |

### Notes

> - Each time we run :bnext (or repeat it with the @: command), it
>   adds a record to the jump list. The (**Ctrl + o**) command goes back to the previous
>   record in the jump list.
> - The (**Ctrl + d**) command asks Vim to reveal a list of possible completions (see
>   :h c_CTRL-D ).