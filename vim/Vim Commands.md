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

## Select

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
| :[range]!{filter}                              | Filter the specified [range] through external program {filter} |
| :[range]write !{cmd}                           | Execute {cmd} in the shell with [range] lines as standard input |
| :read !{cmd}                                   | Execute {cmd} in the shell and insert its standard output<br/>below the cursor |
| :!{cmd}                                        | Execute {cmd} with the shell                                 |
| :shell                                         | Start a shell (return to Vim by typing exit )                |

## Resizing and Rearranging Windows

| Keystrokes        | Buffer Contents                          |
| ----------------- | ---------------------------------------- |
| Ctrl + w + =      | Equalize width and height of all windows |
| Ctrl + w + _      | Maximize height of the active window     |
| Ctrl + w + \|     | Maximize width of the active window      |
| [N] Ctrl + w + _  | Set active window height to [N] rows     |
| [N] Ctrl + w + \| | Set active window width to [N] columns   |

## Moving Around

| Command | Move Cursor                                 |
| ------- | ------------------------------------------- |
| j       | Down one real line                          |
| gj      | Down one display line                       |
| k       | Up one real line                            |
| gk      | Up one display line                         |
| 0       | To first character of real line             |
| g0      | To first character of display line          |
| ^       | To first nonblank character of real line    |
| g^      | To first nonblank character of display line |
| $       | To end of real line                         |
| g$      | To end of display line                      |

## Find based on Character

| Command | Effect                                                       |
| ------- | ------------------------------------------------------------ |
| f{char} | Forward to the next occurrence of {char}                     |
| F{char} | Backward to the previous occurrence of {char}                |
| t{char} | Forward to the character before the next occurrence of {char} |
| T{char} | Backward to the character after the previous occurrence of {char} |
| ;       | Repeat the last character-search command                     |
| ,       | Reverse the last character-search command                    |

## Vim's Automatic Marks

| Keystrokes | Buffer Contents                                   |
| ---------- | ------------------------------------------------- |
| ``         | Position before the last jump within current file |
| `.         | Location of last change                           |
| `^         | Location of last insertion                        |
| `[         | Start of last change or yank                      |
| `]         | End of last change or yank                        |
| `<         | Start of last visual selection                    |
| `>         | End of last visual selection                      |

## Selection of Jumps

| Command                                    | Effect                                         |
| ------------------------------------------ | ---------------------------------------------- |
| [count]G                                   | Jump to line number                            |
| //pattern **CR** / ?pattern **CR** / n / N | Jump to next/previous occurrence of pattern    |
| %                                          | Jump to matching parenthesis                   |
| ( / )                                      | Jump to start of previous/next sentence        |
| { / }                                      | Jump to start of previous/next paragraph       |
| H / M / L                                  | Jump to top/middle/bottom of screen            |
| gf                                         | Jump to file name under the cursor             |
| <C-]>                                      | Jump to definition of keyword under the cursor |
| ’{mark} / `{mark}                          | Jump to a mark                                 |

## Read only registers

| Register | Contents                   |
| -------- | -------------------------- |
| "%       | Name of the current file   |
| "#       | Name of the alternate file |
| ".       | Last inserted text         |
| ":       | Last Ex command            |
| "/       | Last search pattern        |

### Special Characters for Replacement Strings

| Symbol         | Represents                                                   |
| -------------- | ------------------------------------------------------------ |
| \r             | Insert a carriage return                                     |
| \t             | Insert a tab character                                       |
| \\             | Insert a single backslash                                    |
| \1             | Insert the first submatch                                    |
| \2             | Insert the second submatch (and so on, up to \9 )            |
| \0             | Insert the entire matched pattern                            |
| &              | Insert the entire matched pattern                            |
| ~              | Use {string} from the previous invocation of :substitute     |
| \={Vim script} | Evaluate {Vim script} expression; use result as replacement {string} |

### This table summarizes the commands that we can use to navigate our code-base using tags:

| Command          | Effect                                                       |
| ---------------- | ------------------------------------------------------------ |
| <C-]>            | Jump to the first tag that matches the word under the cursor |
| g<C-]>           | Prompt user to select from multiple matches for the word under the cursor. If only one match exists, jump to it without prompting. |
| :tag {keyword}   | Jump to the first tag that matches {keyword}                 |
| :tjump {keyword} | Prompt user to select from multiple matches for {keyword} . If only one match exists, jump to it without prompting. |
| :pop or **C-t ** | Reverse through tag history                                  |
| :tag             | Advance through tag history                                  |
| :tnext           | Jump to next matching tag                                    |
| :tprev           | Jump to previous matching tag                                |
| :tfirst          | Jump to first matching tag                                   |
| :tlast           | Jump to last matching tag                                    |
| :tselect         | Prompt user to choose an item from the tag match list        |

### Commands for Navigating the Quickfix List

| Command | Action                             |
| ------- | ---------------------------------- |
| :cnext  | Jump to next item                  |
| :cprev  | Jump to previous item              |
| :cfirst | Jump to first item                 |
| :clast  | Jump to last item                  |
| :cnfile | Jump to first item in next file    |
| :cpfile | Jump to last item in previous file |
| :cc N   | Jump to nth item                   |
| :copen  | Open the quickfix window           |
| :cclose | Close the quickfix window          |

### Vim's Autocomplete Methods

| Command | Type of Completion      |
| ------- | ----------------------- |
| C-n     | Generic keywords        |
| C-x C-n | Current buffer keywords |
| C-x C-i | Included file keywords  |
| C-x C-] | tags file keywords      |
| C-x C-k | Dictionary lookup       |
| C-x C-l | Whole line completion   |
| C-x C-f | Filename completion     |
| C-x C-o | Omni-completion         |

### Vim Spell Checker's Commands

| Command | Effect                                   |
| ------- | ---------------------------------------- |
| ]s      | Jump to next spelling error              |
| [s      | Jump to previous spelling error          |
| z=      | Suggest corrections for current word     |
| zg      | Add current word to spell file           |
| zw      | Remove current word from spell file      |
| zug     | Revert zg or zw command for current word |

### vim-fugitive commands for vimrc

```bash
" Fugitive Mappings
nnoremap gsl :Glog<CR>
nnoremap gsd :Gdiff<CR>
nnoremap gsb :Gblame<CR>
nnoremap gsw :Gwrite<CR>
nnoremap gsC :Gcommit<CR>
nnoremap gst :Gstatus<CR>
nnoremap gscd :Gcd<Bar>pwd<CR>
nnoremap gsld :Glcd<Bar>pwd<CR>

" Fugitive Commands
command! -bar -nargs=* Gpull execute 'Git pull' <q-args> 'origin' fugitive#head()
command! -bar -nargs=* Gpush execute 'Git push' <q-args> 'origin' fugitive#head()
command! -bar -nargs=* Gpurr execute 'Git pull --rebase' <q-args> 'origin' fugitive#head()
command! Gpnp silent Gpull | Gpush
command! Gprp silent Gpurr | Gpush

command! -bar -nargs=+ -complete=customlist,functions#GitBugComplete Gbug Git bug <q-args>
command! -bar -nargs=+ -complete=customlist,functions#GitFeatureComplete Gfeature Git feature <q-args>
command! -bar -nargs=+ -complete=customlist,functions#GitRefactorComplete Grefactor Git refactor <q-args>

" Fugitive Functions in autoload/functions.vim
function! s:GitShortRefNames(names, full_name) "{{{2
  if a:full_name
    let expr = 'v:val[11:]'
  else
    let expr = 'v:val[strridx(v:val, "/")+1:]'
  endif
  return map(a:names, expr)
endfunction

function! s:GitExecInPath(cmd) "{{{2
  if exists('b:git_dir')
    let path = b:git_dir
  else
    let path = fugitive#extract_git_dir('.')
  endif
  let path = fnamemodify(path, ':h')

  return system('cd ' . path . '; ' . a:cmd)
endfunction

function! s:GitComplete(ArgLead, Cmdline, Cursor, ...) "{{{2
  let refs = 'refs/heads/'
  if a:0 == 1 && a:1 !=? 'branch'
    let refs = 'refs/' . a:1
    let full_name = 1
  elseif a:0 == 2 && a:1 ==? 'branch'
    let refs = refs . a:2
    let full_name = 0
  endif

  let cmd = 'git for-each-ref --format="%(refname)" ' . refs
  if !empty(a:ArgLead)
    let cmd = cmd . ' | sed "s/.*\/\(.*\)/\1/" | grep ^' . a:ArgLead . ' 2>/dev/null'
  endif
  return s:GitShortRefNames(split(s:GitExecInPath(cmd)), full_name)
endfunction

function! s:GitExtraComplete(ArgLead, CmdLine, Cursor, type) "{{{2
  if (empty(a:ArgLead) || a:ArgLead =~? '^f\%[inish]$') && a:CmdLine !~? 'finish\s*$'
    return ['finish']
  else
    return s:GitComplete(a:ArgLead, a:CmdLine, a:Cursor, 'branch', a:type)
  endif
endfunction

function! functions#GitBugComplete(ArgLead, CmdLine, Cursor) "{{{2
  return s:GitExtraComplete(a:ArgLead, a:CmdLine, a:Cursor, 'bug')
endfunction

function! functions#GitFeatureComplete(ArgLead, CmdLine, Cursor) "{{{2
  return s:GitExtraComplete(a:ArgLead, a:CmdLine, a:Cursor, 'feature')
endfunction

function! functions#GitRefactorComplete(ArgLead, CmdLine, Cursor) "{{{2
  return s:GitExtraComplete(a:ArgLead, a:CmdLine, a:Cursor, 'refactor')
endfunction
```

## vimrc 

```
" This is for getting the current buffer filepath in ex-mode
cnoremap <expr> %% getcmdtype() == ':' ? expand('%:h').'/' : '%%'

" The :&& command repeats the last substitute pattern with same flags
nnoremap & :&&<CR>
xnoremap & :&&<CR>

" For populating the Quickfix list with Buffers
command! -nargs=0 -bar Qargs execute 'args' QuickfixFilenames()
function! QuickfixFilenames()
let buffer_numbers = {}
for quickfix_item in getqflist()
let buffer_numbers[quickfix_item['bufnr']] = bufname(quickfix_item['bufnr'])
endfor
return join(map(values(buffer_numbers), 'fnameescape(v:val)'))
endfunction
```

### Notes

> - Each time we run :bnext (or repeat it with the @: command), it
>   adds a record to the jump list. The (**Ctrl + o**) command goes back to the previous
>   record in the jump list.
> - The (**Ctrl + d**) command asks Vim to reveal a list of possible completions (see
>   :h c_CTRL-D ).
> - **[(Ctrl + w) w]** => Cycle between open windows
> - **Ctrl + w + T** Move the current window into its own tab
> - **qA** will append the macros what we have stored in the **a** register

