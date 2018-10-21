# Vim Commands

| ID   | MODE                                                         |                         COMMAND                          | DESCRIPTION                                                  |
| :--- | :----------------------------------------------------------- | :------------------------------------------------------: | :----------------------------------------------------------- |
| 3610 | Move left and right                                          |                           N h                            | Move N digits to the left (same for CTRL - H, <BS>, <Left> keys) |
| 3611 | Move left and right                                          |                           N l                            | Move N digits to the right (same for <Space>, <Right> keys)  |
| 3612 | Move left and right                                          |                            0                             | Move to beginning of line (same as <Home> key)               |
| 3613 | Move left and right                                          |                            ^                             | Move to the beginning of a line (except for white space characters) |
| 3614 | Move left and right                                          |                           N $                            | Move to the end of the line.  (N-1 line, move down) (same for <End> key) |
| 3615 | Move left and right                                          |                           g 0                            | Move to the beginning of the line on the screen.  (The movement when crossing over multiple lines is different from "0") |
| 3616 | Move left and right                                          |                           g ^                            | Move to the beginning of the line on the screen (except for white space characters).  (The movement when crossing over multiple lines is different from "^") |
| 3617 | Move left and right                                          |                          N g $                           | Move to the end of the line.  (The movement when crossing over multiple lines is different from "$") |
| 3618 | Move left and right                                          |                            gm                            | Move to the center of the current line (half of the width of the terminal) |
| 3619 | Move left and right                                          |                           N \|                           | Move to Nth digit.  (Default is 1)                           |
| 3620 | Move left and right                                          |                        N f {char}                        | Move to the Nth {char} in the right direction from the current position |
| 3621 | Move left and right                                          |                        NF {char}                         | Move to the Nth {char} in the left direction from the current position |
| 3622 | Move left and right                                          |                        N t {char}                        | Move to the left of the Nth {char} in the right direction from the current position |
| 3623 | Move left and right                                          |                        NT {char}                         | Move to the right of the Nth {char} in the left direction from the current position |
| 3624 | Move left and right                                          |                            N;                            | Repeat the last "f", "F", "t", "T" N times.                  |
| 3625 | Move left and right                                          |                            N,                            | Repeat the last "f", "F", "t", "T" N times in the reverse direction. |
| 3626 | Move up and down                                             |                           N k                            | Move up N lines (same for CTRL-P, <Up> key)                  |
| 3627 | Move up and down                                             |                           N j                            | Move N lines down (same for CTRL-J, CTRL-N, <NL>, <Down>)    |
| 3628 | Move up and down                                             |                           N -                            | Move up N lines and move to non-whitespace at the beginning of the line |
| 3629 | Move up and down                                             |                           N +                            | Move down N lines and move to non-blank character at the beginning of line (same with CTRL-M, <CR> key) |
| 3630 | Move up and down                                             |                           N _                            | Move down N-1 lines and move to the non-blank character at the beginning of the line |
| 3631 | Move up and down                                             |                            NG                            | Move to the Nth line (default is the last line) and move to the non-blank character at the beginning of the line |
| 3632 | Move up and down                                             |                           N gg                           | Move to the Nth line (default is the 1st line) and move to the non-blank character at the beginning of the line |
| 3633 | Move up and down                                             |                            N%                            | Move to the Nth percentile of the file.  N must be specified for this command.  If not specified, \|% \| command handling. |
| 3634 | Move up and down                                             |                           N gk                           | Move N rows up on the screen.  (The movement when there is a line spanning multiple lines is different from "k") |
| 3635 | Move up and down                                             |                           N gj                           | Move N rows down on the screen.  (If there is a line that spans multiple lines |
| 3636 | Moving text context unit                                     |                           N w                            | Proceed for the Nth word                                     |
| 3637 | Moving text context unit                                     |                            NW                            | Go forward by N words (= \| WORD \|) separated by whitespace |
| 3638 | Moving text context unit                                     |                           N e                            | Proceed to the bottom of Nth word                            |
| 3639 | Moving text context unit                                     |                            NE                            | Words separated by whitespace (= \| WORD \|) Proceed to N th hips |
| 3640 | Moving text context unit                                     |                           N b                            | Back to the previous N words                                 |
| 3641 | Moving text context unit                                     |                            NB                            | Words separated by white space (= \| WORD \|) N back, back   |
| 3642 | Moving text context unit                                     |                           N ge                           | Back to the bottom of Nth word                               |
| 3643 | Moving text context unit                                     |                           N gE                           | Words separated by white space (= \| WORD \|) Return to N's hips |
| 3644 | Moving text context unit                                     |                            N)                            | N sentences (sentences) minutes, go ahead                    |
| 3645 | Moving text context unit                                     |                           N (                            | N sentences, back to previous                                |
| 3646 | Moving text context unit                                     |                            N}                            | Advance by N paragraphs (paragraph)                          |
| 3647 | Moving text context unit                                     |                           N {                            | N paragraph minutes back                                     |
| 3648 | Moving text context unit                                     |                           N]]                            | Move forward by N sections (chapter), move forward           |
| 3649 | Moving text context unit                                     |                           N [[                           | N sections (chapters) minutes back, move to the beginning    |
| 3650 | Moving text context unit                                     |                           N] [                           | Go forward to N section (chapter) minutes, move to the end   |
| 3651 | Moving text context unit                                     |                           N []                           | N sections (chapters) minutes back, move to the end          |
| 3652 | Moving text context unit                                     |                           N [(                           | Go back to the 'N' not responding '('                        |
| 3653 | Moving text context unit                                     |                           N [{                           | Go back to the '{' 'not responding to the N th               |
| 3654 | Moving text context unit                                     |                           N [m                           | Return to the beginning of N previous methods (for Java)     |
| 3655 | Moving text context unit                                     |                           N [M                           | Return to the end of N previous methods (for Java)           |
| 3656 | Moving text context unit                                     |                           N])                            | Proceed to N 'not responding') '                             |
| 3657 | Moving text context unit                                     |                           N]}                            | Proceed to 'N' not responding '}'                            |
| 3658 | Moving text context unit                                     |                           N] m                           | Proceed to the beginning of the N-th method (for Java)       |
| 3659 | Moving text context unit                                     |                           N] M                           | Proceed to the end of the N-th method (for Java)             |
| 3660 | Moving text context unit                                     |                           N [#                           | Return to the Nth unresponsive "#if" or "#else"              |
| 3661 | Moving text context unit                                     |                           N] #                           | Proceed to "#else" or "#endif" that is not corresponding to Nth |
| 3662 | Moving text context unit                                     |                           N [*                           | Back to the beginning of N previous comments                 |
| 3663 | Moving text context unit                                     |                           N] *                           | Proceed to the end of N next comments                        |
| 3664 | Pattern search                                               |             N / {pattern} [/ [offset]] <CR>              | Search downward to the point containing the Nth {pattern}    |
| 3665 | Pattern search                                               |              N? {Pattern} [? [Offset]] <CR>              | Search upward for the part containing the Nth {pattern}      |
| 3666 | Pattern search                                               |                         N / <CR>                         | Search under the same condition as before is performed for the downward direction |
| 3667 | Pattern search                                               |                         N? <CR>                          | Search in the same condition as before is performed for upward direction |
| 3668 | Pattern search                                               |                           N n                            | Re-execute previous search                                   |
| 3669 | Pattern search                                               |                            NN                            | Re-execute the previous search in the reverse direction      |
| 3670 | Pattern search                                               |                           N *                            | Search words located at the cursor downward                  |
| 3671 | Pattern search                                               |                           N #                            | Search words located at the cursor upward                    |
| 3672 | Pattern search                                               |                          N g *                           | Same as "*" but search for partial match                     |
| 3673 | Pattern search                                               |                          N g #                           | Same as "#", but search for partial match                    |
| 3674 | Pattern search                                               |                            gd                            | Move to locale declaration of cursor position identifier     |
| 3675 | Pattern search                                               |                            gD                            | Move to the global declaration of the identifier at the cursor position |
| 3676 | mark                                                         |                      m {a - zA - Z}                      | Mark current location as {a-zA-Z}                            |
| 3677 | mark                                                         |                          `{az}                           | Move to the mark {az} of the file being edited               |
| 3678 | mark                                                         |                          `{AZ}                           | Move to mark of arbitrary file {AZ}                          |
| 3679 | mark                                                         |                          `{0-9}                          | Move to where vim last time                                  |
| 3680 | mark                                                         |                            ``                            | Move to the location before the previous jump command        |
| 3681 | mark                                                         |                            `"                            | Move to the location of the last time you edited this file   |
| 3682 | mark                                                         |                            `[                            | Move to the beginning of the character string which was repeated or pasted just before |
| 3683 | mark                                                         |                            `]                            | Move to the end of the character string which was cropped or put just before |
| 3684 | mark                                                         |                            `<                            | Move to the beginning of (previous) visual area              |
| 3685 | mark                                                         |                            `>                            | Move to the end of (previous) visual area                    |
| 3686 | mark                                                         |                            `.                            | Move to the last change in this file                         |
| 3687 | mark                                                         |               '{a - zA - Z 0 - 9 []' "<>.}               | `, Except that it moves to the first non-blank character of the line. |
| 3688 | mark                                                         |                         : marks                          | List currently set marks                                     |
| 3689 | mark                                                         |                         N CTRL-O                         | Move to the Nth oldest place in the jump list                |
| 3690 | mark                                                         |                         N CTRL-I                         | Move to the Nth new place in the jump list                   |
| 3691 | mark                                                         |                        : ju [mps]                        | List jump list                                               |
| 3692 | Miscellaneous movement commands                              |                            %                             | Search for pairs of corresponding brackets ("(", "[", "{"), comments, "# if" / "# else" / "# endif" |
| 3693 | Miscellaneous movement commands                              |                            NH                            | Move to the first non-blank character on the Nth line on the screen |
| 3694 | Miscellaneous movement commands                              |                            M                             | Move to the first non-blank character in the middle row on the screen |
| 3695 | Miscellaneous movement commands                              |                            NL                            | Move to the first non-blank character on the Nth line from the bottom on the screen |
| 3696 | Miscellaneous movement commands                              |                           N go                           | Move to the Nth byte of the current buffer                   |
| 3697 | Miscellaneous movement commands                              |                 : [range] go [to] [off]                  | Move to [off] byte of current buffer                         |
| 3698 | Using tags                                                   |                    : ta [g] [!] {tag}                    | Jump to the tag specified by {tag}                           |
| 3699 | Using tags                                                   |                   : [count] ta [g] [!]                   | Jump to the tag [count] th new tag                           |
| 3700 | Using tags                                                   |                          CTRL-]                          | Jump to the tag at the cursor position unless changed        |
| 3701 | Using tags                                                   |                  : ts [elect] [!] [tag]                  | Display the list that matches the tag, select the jump destination |
| 3702 | Using tags                                                   |                   : tj [ump] [!] [tag]                   | Jump to specified tag [tag].  If there are multiple matching tags, select from the list |
| 3703 | Using tags                                                   |                   : lt [ag] [!] [tag]                    | Jump to tag [tag] and add matched tag to location list.      |
| 3704 | Using tags                                                   |                          : tags                          | List tag list                                                |
| 3705 | Using tags                                                   |                         N CTRL-T                         | Jump to the Nth oldest tag in the tag list                   |
| 3706 | Using tags                                                   |                   : [count] po [p] [!]                   | Jump to the [count] th oldest tag in the tag list            |
| 3707 | Using tags                                                   |                  : [count] tn [ext] [!]                  | [count] jump to the next tag                                 |
| 3708 | Using tags                                                   |                : [count] tp [revious] [!]                | Jump to the previous tag for [count] pieces                  |
| 3709 | Using tags                                                   |             : [count] tr [ewind] [!] [count]             | Jump to the second matching tag                              |
| 3710 | Using tags                                                   |                      : tl [ast] [!]                      | Jump to the last matched tag                                 |
| 3711 | Using tags                                                   |                     : pt [ag] {tag}                      | {tag} Open the preview screen for viewing tags               |
| 3712 | Using tags                                                   |                        CTRL - W}                         | It is the same as CTRL-] but jumps to the preview screen     |
| 3713 | Using tags                                                   |                      : pts [elect]                       | Just like ": tselect" but jump to the preview screen         |
| 3714 | Using tags                                                   |                       : ptj [ump]                        | Just like ": tjump" but jump to the preview screen           |
| 3715 | Using tags                                                   |                       : pc [lose]                        | Close the tag preview screen.                                |
| 3716 | Using tags                                                   |                         CTRL-W z                         | Close the tag preview screen.                                |
| 3717 | scroll                                                       |                         N CTRL-E                         | Scroll the screen down by N lines downward (default is 1)    |
| 3718 | scroll                                                       |                         N CTRL-D                         | Scroll the screen down by N lines downward (default is half of screen) |
| 3719 | scroll                                                       |                         N CTRL-F                         | Scroll down the screen by N pages                            |
| 3720 | scroll                                                       |                         N CTRL-Y                         | Scroll upward by N rows of the screen (default is 1)         |
| 3721 | scroll                                                       |                         N CTRL-U                         | Scroll the screen upward by N lines (default is half of the screen) |
| 3722 | scroll                                                       |                         N CTRL-B                         | Scroll the screen upward by N pages                          |
| 3723 | scroll                                                       |                       z <CR> or zt                       | Make the current line the first line of the screen and redraw |
| 3724 | scroll                                                       |                            z.                            | or zz Make the current line the center of the screen and redraw |
| 3725 | scroll                                                       |                            z-                            | or zb Make the current line the bottom line of the screen and redraw |
| 3726 | Valid only when 'wrap' is off                                |                           N zh                           | Scroll the screen N characters, scroll to the right          |
| 3727 | Valid only when 'wrap' is off                                |                           N zl                           | Screen N characters, scroll to the left                      |
| 3728 | Valid only when 'wrap' is off                                |                          N z H                           | Scroll right by half of screen length                        |
| 3729 | Valid only when 'wrap' is off                                |                           N zL                           | Scroll to the left by half of the screen length              |
| 3730 | Insert string                                                |                           N a                            | Add character string (N times) after cursor position         |
| 3731 | Insert string                                                |                            NA                            | Add a character string (N times) to the end of the current line |
| 3732 | Insert string                                                |                           N i                            | Add character string (N times) before cursor position (same as <Insert>) |
| 3733 | Insert string                                                |                            NI                            | Add character string (N times) before the first non-blank character of the current line |
| 3734 | Insert string                                                |                          N g I                           | Add a character string (N times) to the beginning of the current line |
| 3735 | Insert string                                                |                            No                            | Add a new line below the current line and add a character string (N times). |
| 3736 | Insert string                                                |                            No                            | Insert a new line in the current line and add a character string (N times). |
| 3737 | Insert string                                                |                   : star [tinsert] [!]                   | Start Insert mode.  Specifying [!] Puts into Append mode.    |
| 3738 | Insert string                                                |                  : startr [eplace] [!]                   | Start Replace mode.  Specifying [!] Starts at the end of the line. |
| 3739 | Visual mode                                                  |                            I                             | Insert the same character string before all the selected lines. |
| 3740 | Visual mode                                                  |                            A                             | Insert the same character string after all selected lines.   |
| 3741 | End insert mode                                              |                          <Esc>                           | End the insertion mode and return to normal mode             |
| 3742 | End insert mode                                              |                          CTRL-C                          | Same as <Esc>.  However, abbreviations are not developed     |
| 3743 | End insert mode                                              |                     CTRL-O {command}                     | Execute {command} and return to insert mode                  |
| 3744 | Move                                                         |                       cursor keys                        | Move the cursor up, down, left and right                     |
| 3745 | Move                                                         |                    shift-left / right                    | Move one word horizontally by one word                       |
| 3746 | Move                                                         |                     shift-up / down                      | Move backward and forward for each screen                    |
| 3747 | Move                                                         |                          <End>                           | Move to the last digit of the line                           |
| 3748 | Move                                                         |                          <Home>                          | Move to the first digit of the line                          |
| 3749 | Special key in insert mode                                   |                     CTRL-V {char} ..                     | Insert specified {char}, or decimal byte value               |
| 3750 | Special key in insert mode                                   |             <NL> or <CR> or CTRL-M or CTRL-J             | Break a line and create a new line                           |
| 3751 | Special key in insert mode                                   |                          CTRL-E                          | Insert one character of the line immediately under the cursor position |
| 3752 | Special key in insert mode                                   |                          CTRL-Y                          | Insert the contents of the line just above the cursor position one character |
| 3753 | Special key in insert mode                                   |                          CTRL-A                          | Insert the last inserted string again                        |
| 3754 | Special key in insert mode                                   |                         CTRL- @                          | Insert the last inserted character string and return from insert mode |
| 3755 | Special key in insert mode                                   |            CTRL - R {0 - 9 a - z% #:. - = "}             | Insert contents of specified register                        |
| 3756 | Special key in insert mode                                   |                          CTRL-N                          | Inspect by inserting words that match the keyword in front of the cursor in the forward direction |
| 3757 | Special key in insert mode                                   |                          CTRL-P                          | Insert a word matching the keyword in front of the cursor in reverse direction |
| 3758 | Special key in insert mode                                   |                        CTRL-X ...                        | Complement words in front of the cursor in various ways.     |
| 3759 | Special key in insert mode                                   |                      <BS> or CTRL-H                      | Delete one character before the cursor                       |
| 3760 | Special key in insert mode                                   |                          <Del>                           | Delete one character at the cursor position                  |
| 3761 | Special key in insert mode                                   |                          CTRL-W                          | Delete one word at cursor position                           |
| 3762 | Special key in insert mode                                   |                          CTRL-U                          | Delete all characters entered on the current line            |
| 3763 | Special key in insert mode                                   |                          CTRL-T                          | Insert the specified amount of 'shiftwidth' at the beginning of the current line |
| 3764 | Special key in insert mode                                   |                          CTRL-D                          | Delete the specified indent of 'shiftwidth' from the beginning of the current line |
| 3765 | Special key in insert mode                                   |                         0 CTRL-D                         | Delete all indent of current line                            |
| 3766 | Special key in insert mode                                   |                         ^ CTRL-D                         | Delete all indentation of the current line.  However, it does not affect indentation of the next line. |
| 3767 | Special insert command                                       |                        : r [file]                        | Insert the contents of [file] after the cursor position      |
| 3768 | Special insert command                                       |                      : r! {command}                      | Insert the contents of the standard output as a result of executing {command} after the cursor position |
| 3769 | Delete string                                                |                           N x                            | Delete cursor position and N characters after it             |
| 3770 | Delete string                                                |                         N <Del>                          | Delete cursor position and N characters after it             |
| 3771 | Delete string                                                |                            NX                            | Delete N characters before cursor position                   |
| 3772 | Delete string                                                |                       N d {motion}                       | Delete the character string in the range specified by {motion} |
| 3773 | Delete string                                                |                        {visual} d                        | Delete highlighted character string                          |
| 3774 | Delete string                                                |                           N dd                           | Delete N lines                                               |
| 3775 | Delete string                                                |                            ND                            | Delete until the end of the line (after N-1 line)            |
| 3776 | Delete string                                                |                            NJ                            | Combine N-1 lines and put on one line (delete <EOL>)         |
| 3777 | Delete string                                                |                        {visual} J                        | Combine selected character strings in visual mode            |
| 3778 | Delete string                                                |                           N gJ                           | Same as "J", but do not put a space between the lines        |
| 3779 | Delete string                                                |                       {visual} gJ                        | "Same as {visual} J", but do not put a space between the lines |
| 3780 | Delete string                                                |                     : [range] d [x]                      | Delete line in the range specified by [range] [to register x it] |
| 3781 | Copying and Moving a String                                  |                         "{char}                          | Specify register {char}.  Following this, specify delete command, yank command, put command |
| 3782 | Copying and Moving a String                                  |                          : reg                           | Display contents of all registers                            |
| 3783 | Copying and Moving a String                                  |                       : reg {arg}                        | Display contents of register indicated by {arg}              |
| 3784 | Copying and Moving a String                                  |                       N y {motion}                       | Yank (copy) the character string in the range specified by {motion} |
| 3785 | Copying and Moving a String                                  |                        {visual} y                        | Yank the register to highlighted character string            |
| 3786 | Copying and Moving a String                                  |                           N yy                           | Y row in register to register Y                              |
| 3787 | Copying and Moving a String                                  |                            NY                            | Y row in register to register Y                              |
| 3788 | Copying and Moving a String                                  |                           N p                            | Put the register contents N times after the cursor position (paste) |
| 3789 | Copying and Moving a String                                  |                            NP                            | Put the register contents N times before the cursor position (paste) |
| 3790 | Copying and Moving a String                                  |                           N] p                           | It is the same as p, but it is indented to the current line  |
| 3791 | Copying and Moving a String                                  |                           N [p                           | It is the same as P, but it is indented to the current line  |
| 3792 | Copying and Moving a String                                  |                           N gp                           | Same as p but moving the cursor after the inserted character string |
| 3793 | Copying and Moving a String                                  |                          N g P                           | It is the same as P, but moves the cursor after the inserted character string |
| 3794 | "Change" means to delete the character string and enter the insertion mode |                       N c {motion}                       | Change the character string in the range specified by {motion} |
| 3795 | "Change" means to delete the character string and enter the insertion mode |                        {visual} c                        | Change selected character string in visual mode              |
| 3796 | "Change" means to delete the character string and enter the insertion mode |                           N cc                           | Change N lines                                               |
| 3797 | "Change" means to delete the character string and enter the insertion mode |                            NS                            | Change N lines                                               |
| 3798 | "Change" means to delete the character string and enter the insertion mode |                            NC                            | Change to the end of the line (after N-1 line)               |
| 3799 | "Change" means to delete the character string and enter the insertion mode |                           N s                            | Change N letters                                             |
| 3800 | Change string                                                |                        N r {char}                        | Replace N characters with {char}                             |
| 3801 | Change string                                                |                       N gr {char}                        | Replace N characters without affecting layout                |
| 3802 | Change string                                                |                            NR                            | To replace mode (Repeat input character string N times)      |
| 3803 | Change string                                                |                           N gR                           | Go to virtual replacement mode.  It is the same as the replacement mode, but it does not affect the layout. |
| 3804 | Change string                                                |                    {visual} r {char}                     | For visual block mode: Replace each character in the selected range with {char}, substitute |
| 3805 | Change string                                                |                        {visual} c                        | For visual block mode: Replace the contents of each selected line with the input character string |
| 3806 | Change string                                                |                        {visual} C                        | For visual block mode: Replace with the input string up to the end of each line of each selected line |
| 3807 | Change string                                                |                           N ~                            | Convert N letters of uppercase / lowercase letters and move the cursor |
| 3808 | Change string                                                |                        {visual} ~                        | Convert uppercase / lowercase letters in the selected range in visual mode |
| 3809 | Change string                                                |                        {visual} u                        | Convert selected range in lower right letters in visual mode |
| 3810 | Change string                                                |                        {visual} U                        | Convert selected range in upper case to uppercase in visual mode |
| 3811 | Change string                                                |                       g ~ {motion}                       | Convert uppercase / lowercase letters in the range specified by {motion} |
| 3812 | Change string                                                |                       gu {motion}                        | Convert the range specified by {motion} to lower case        |
| 3813 | Change string                                                |                       gU {motion}                        | Convert the range specified by {motion} to upper case        |
| 3814 | Change string                                                |                       {visual} g?                        | Encode the range selected in visual mode with rot13.         |
| 3815 | Change string                                                |                       g? {motion}                        | Encode the range specified by {motion} with rot13.           |
| 3816 | Change string                                                |                         N CTRL-A                         | Add N to the cursor position or the number behind            |
| 3817 | Change string                                                |                         N CTRL-X                         | Subtract N from the cursor position or the number behind     |
| 3818 | Change string                                                |                       N <{motion}                        | Reduce indent by 'shiftwidth' for the range specified by {motion} |
| 3819 | Change string                                                |                           N <<                           | Reduce the indent of N lines from the current line           |
| 3820 | Change string                                                |                       N> {motion}                        | Increase indent by 'shiftwidth' by the range specified by {motion} |
| 3821 | Change string                                                |                           N >>                           | Increase the indent of N lines from the current line         |
| 3822 | Change string                                                |                      N gq {motion}                       | Formats the range specified by {motion} to the length specified by 'textwidth' |
| 3823 | Change string                                                |                   : [range] ce [nter]                    | [width] Center line range of [range]                         |
| 3824 | Change string                                                |                    : [range] le [ft]                     | [indent] Left line range of [range] ((indent) minutes)       |
| 3825 | Change string                                                |                    : [range] ri [ght]                    | [width] Right-justify the range of [range] (up to [width] digits) |
| 3826 | Complex change processing                                    |                N! {Motion} {command} <CR>                | Replace the range specified by {motion} with the result output of {command} |
| 3827 | Complex change processing                                    |                   N !! {command} <CR>                    | Replace N lines with output of {command}                     |
| 3828 | Complex change processing                                    |                 {visual}! {command} <CR>                 | Replace the selected range in visual mode with the result output of {command} |
| 3829 | Complex change processing                                    |                : [range]! {command} <CR>                 | Replace the range of [range] with the result output of {command} |
| 3830 | Complex change processing                                    |                       N = {motion}                       | Replace the range specified by {motion} with the result output of 'equalprg' |
| 3831 | Complex change processing                                    |                           N ==                           | Replace N lines with the result output of 'equalprg'         |
| 3832 | Complex change processing                                    |                        {visual} =                        | Replace the selected range in visual mode with the result output of 'equalprg' |
| 3833 | Complex change processing                                    | : [range] s [ubstitute] / {pattern} / {string} / [g] [c] | Replace {pattern} in the range of [range] with {string}.  Specifying [g] replaces all {pattern} found.  When [c] is specified, each substitution is confirmed. |
| 3834 | Complex change processing                                    |             : [range] s [ubstitute] [g] [c]              | Repeat last ": s" with new range and option                  |
| 3835 | Complex change processing                                    |                            &                             | Repeat last ": s" for the current line.  (No option)         |
| 3836 | Complex change processing                                    |             : [range] ret [ab] [!] [tabstop]             | Change the value of 'tabstop' and make whitespace, TAB sorts accordingly accordingly. |
| 3837 | Visual mode                                                  |                            v                             | Start character mode visual mode} Move the cursor            |
| 3838 | Visual mode                                                  |                            V                             | Start visual mode on a line basis} For the selected range    |
| 3839 | Visual mode                                                  |                          CTRL-V                          | Run rectangular unit visual mode} command                    |
| 3840 | Visual mode                                                  |                            o                             | Swap the cursor position and start position of selection range |
| 3841 | Visual mode                                                  |                            gv                            | Start the visual mode with the previous selected range selected |
| 3842 | String object (in visual mode or after operator specification) |                           N aw                           | Select "a word" (also delete spaces before and after the word) |
| 3843 | String object (in visual mode or after operator specification) |                           N iw                           | Select "inner word" (delete only the net words)              |
| 3844 | String object (in visual mode or after operator specification) |                           N aW                           | Select "a \| WORD \|"                                        |
| 3845 | String object (in visual mode or after operator specification) |                           N iW                           | Select "inner \| WORD \|"                                    |
| 3846 | String object (in visual mode or after operator specification) |                           N as                           | Select "a sentence"                                          |
| 3847 | String object (in visual mode or after operator specification) |                           N is                           | Select "inner sentence"                                      |
| 3848 | String object (in visual mode or after operator specification) |                           N ap                           | Select "a paragraph"                                         |
| 3849 | String object (in visual mode or after operator specification) |                           N ip                           | Select "inner paragraph"                                     |
| 3850 | String object (in visual mode or after operator specification) |                           N ab                           | Select "a block" ("[(" ~ "))" range)                         |
| 3851 | String object (in visual mode or after operator specification) |                           N ib                           | Select "inner block" ("[(" ~ "))" range)                     |
| 3852 | String object (in visual mode or after operator specification) |                          N a B                           | Select "a Block" ("[{" ~ "]}" range)                         |
| 3853 | String object (in visual mode or after operator specification) |                          N i B                           | Select "inner Block" ("[{" ~ "}}" range)                     |
| 3854 | String object (in visual mode or after operator specification) |                           N a>                           | Select "a <> block"                                          |
| 3855 | String object (in visual mode or after operator specification) |                           N i>                           | Select "inner <> block"                                      |
| 3856 | String object (in visual mode or after operator specification) |                           N at                           | Select "a tag block" (<aaa> ~ </ aaa>)                       |
| 3857 | String object (in visual mode or after operator specification) |                           N it                           | Select "inner tag block" (<aaa> ~ </ aaa>)                   |
| 3858 | String object (in visual mode or after operator specification) |                          N a '                           | Select "a single quoted string"                              |
| 3859 | String object (in visual mode or after operator specification) |                          N i '                           | Select "inner single quoted string"                          |
| 3860 | String object (in visual mode or after operator specification) |                          N a "                           | Select "a double quoted string"                              |
| 3861 | String object (in visual mode or after operator specification) |                          N i "                           | Select "inner double quoted string"                          |
| 3862 | String object (in visual mode or after operator specification) |                          N a '                           | Select "a backward quoted string"                            |
| 3863 | String object (in visual mode or after operator specification) |                          N i '                           | Select "inner backward quoted string"                        |
| 3864 | Repeat command                                               |                            N.                            | Repeat the previous command.  (The number of times is N)     |
| 3865 | Repeat command                                               |                          q {az}                          | Record the entered character group in register {az}          |
| 3866 | Repeat command                                               |                          q {AZ}                          | Add the input character group to the register {az} and record it |
| 3867 | Repeat command                                               |                            q                             | End recording                                                |
| 3868 | Repeat command                                               |                         N @ {az}                         | Execute the contents of register {az} N times                |
| 3869 | Repeat command                                               |                          N @ @                           | Execute the last @ {az} N times                              |
| 3870 | Repeat command                                               |                         : @ {az}                         | Execute N times by assuming the contents of register {az} as Ex command |
| 3871 | Repeat command                                               |                          : @ @                           | Last: Execute @ {az} N times                                 |
| 3872 | Repeat command                                               |         : [range] g [lobal] / {pattern} / [cmd]          | In [range], execute the [cmd] command (": p" by default) for each line that matches the specified {pattern}. |
| 3873 | Repeat command                                               |         : [range] g [lobal]! / {pattern} / [cmd]         | Do not match the specified {pattern} in [range] ** Execute the [cmd] command (": p" by default) for each line. |
| 3874 | Repeat command                                               |                    : so [urce] {file}                    | Read Ex command from {file}.                                 |
| 3875 | Repeat command                                               |                   : so [urce]! {file}                    | Read the vim command from {file}.                            |
| 3876 | Repeat command                                               |                     : sl [eep] [sec]                     | [sec] Do nothing during the interval                         |
| 3877 | Repeat command                                               |                           N gs                           | I do not do anything for N seconds                           |
| 3878 | Undo / Redo command                                          |                           N u                            | Undo the last N tasks                                        |
| 3879 | Undo / Redo command                                          |                         N CTRL-R                         | Cancel last N undo (redo)                                    |
| 3880 | Undo / Redo command                                          |                            U                             | Cancel changes to the entire line                            |
| 3881 | External command                                             |                        : sh [ell]                        | Start the shell                                              |
| 3882 | External command                                             |                       :! {command}                       | Start {shell} in shell                                       |
| 3883 | External command                                             |                            K                             | Examine the word under the cursor with the 'keywordprg' external command.  (The default is "man") |
| 3884 | Various commands                                             |                          CTRL-L                          | Repaint the screen                                           |
| 3885 | Various commands                                             |                          CTRL-G                          | Display current (path name +) file name and cursor position  |
| 3886 | Various commands                                             |                            ga                            | Display ASCII character code of cursor position in decimal, hexadecimal, octal |
| 3887 | Various commands                                             |                            g8                            | For utf-8 encoding: Display the byte sequence of characters under the cursor in hexadecimal. |
| 3888 | Various commands                                             |                         g CTRL-G                         | Display number of cursor digits, number of lines, number of words, number of characters |
| 3889 | Various commands                                             |                          CTRL-C                          | Searching: Canceling search                                  |
| 3890 | Various commands                                             |                        CTRL-Break                        | MS-DOS: Searching: Canceling search                          |
| 3891 | Various commands                                             |                          <Del>                           | Specifying count: Remove last character                      |
| 3892 | Various commands                                             |                       : ve [rsion]                       | Display version information                                  |
| 3893 | Various commands                                             |                    : mode N MS - DOS:                    | Set the screen mode to N (numbers, C80, C4350, etc.)         |
| 3894 | Various commands                                             |                     : norm [al] [!]                      | {commands} Execute normal mode command                       |
| 3895 | Various commands                                             |                            Q                             | Transition to "Ex" mode                                      |
| 3896 | Various commands                                             |                     : redir> {file}                      | Redirect message to {file}                                   |
| 3897 | Various commands                                             |                  : silent [!] {command}                  | Execute {command} silently                                   |
| 3898 | Various commands                                             |                   : confirm {command}                    | Confirm changes that have not been saved, read-only, etc. when exiting, saving, etc. |
| 3899 | Various commands                                             |                    : browse {command}                    | Use the selection dialog screen when opening or saving a file. |
| 3900 | Edit command line                                            |                          <Esc>                           | Discard the command line (press twice if 'wildchar' is <Esc>) |
| 3901 | Edit command line                                            |                      CTRL-V {char}                       | Insert {char} as a character (CTRL character, etc.)          |
| 3902 | Edit command line                                            |                     CTRL-V {number}                      | Enter the character code in decimal (up to 3 digits)         |
| 3903 | Edit command line                                            |             CTRL - R {0 - 9 a - z "% #: - =}             | Insert register contents                                     |
| 3904 | Edit command line                                            |                     <Left> / <Right>                     | Move cursor left and right                                   |
| 3905 | Edit command line                                            |                   <S-Left> / <S-Right>                   | Move the cursor left or right word by word                   |
| 3906 | Edit command line                                            |                     CTRL-B / CTRL-E                      | Move the cursor to the beginning of a line, move to the end of a line |
| 3907 | Edit command line                                            |                           <BS>                           | Delete the character immediately before the cursor           |
| 3908 | Edit command line                                            |                          <Del>                           | Delete character at cursor position                          |
| 3909 | Edit command line                                            |                          CTRL-W                          | Delete the character immediately before the cursor           |
| 3910 | Edit command line                                            |                          CTRL-U                          | Delete all characters                                        |
| 3911 | Edit command line                                            |                      <Up> / <Down>                       | Invoke the command line history starting with the current command |
| 3912 | Edit command line                                            |                    <S-Up> / <S-Down>                     | Call command line history                                    |
| 3913 | Edit command line                                            |                       : his [tory]                       | Display command line history                                 |
| 3914 | Command line editing / context dependent completion function |                          CTRL-D                          | Display a list of all names that match the pattern immediately before the current cursor |
| 3915 | Command line editing / context dependent completion function |                          CTRL-A                          | Insert all names matching the pattern immediately before the current cursor |
| 3916 | Command line editing / context dependent completion function |                          CTRL-L                          | Insert the common part of those matching the pattern immediately before the current cursor |
| 3917 | Range of Ex command                                          |                            ,                             | Range of two rows                                            |
| 3918 | Range of Ex command                                          |                            ;                             | Same as above.  From the first designated line to the next specified range |
| 3919 | Range of Ex command                                          |                         {number}                         | Line number in file                                          |
| 3920 | Range of Ex command                                          |                            .                             | Current line                                                 |
| 3921 | Range of Ex command                                          |                            $                             | Last line of file                                            |
| 3922 | Range of Ex command                                          |                            %                             | 1, Same as $ (= whole file)                                  |
| 3923 | Range of Ex command                                          |                            *                             | Same as '<,'> (= selection range of visual mode)             |
| 3924 | Range of Ex command                                          |                            t                             | Row of mark t                                                |
| 3925 | Range of Ex command                                          |                     / {pattern} [/]                      | The line following the line matching {pattern}               |
| 3926 | Range of Ex command                                          |                     ? {pattern} [?]                      | The line before the line matching {pattern}                  |
| 3927 | Range of Ex command                                          |                         + [num]                          | The previous line specification (default: 1) plus [num]      |
| 3928 | Range of Ex command                                          |                         - [num]                          | Subtract [num] from previous line specification (default: 1) |
| 3929 | Special Ex characters                                        |                            \|                            | Split command into two (not available for ": global" and ":!") |
| 3930 | Special Ex characters                                        |                            "                             | Start comment                                                |
| 3931 | Special Ex characters                                        |                            %                             | Current file name (only available where file names should be used) |
| 3932 | Special Ex characters                                        |                         # [num]                          | Another file name [num] (only in places where file names should be used) |
| 3933 | If it is present: Discard changes to the current buffer and execute command |                   : e [dit] [!] {file}                   | Edit {file}                                                  |
| 3934 | If it is present: Discard changes to the current buffer and execute command |                      : e [dit] [!]                       | Reload current buffer contents                               |
| 3935 | If it is present: Discard changes to the current buffer and execute command |                      : ene [w] [!]                       | Edit new unnamed buffer                                      |
| 3936 | If it is present: Discard changes to the current buffer and execute command |                   : fin [d] [!] {file}                   | Search {file} from 'path' and edit                           |
| 3937 | File editing                                                 |                        N CTRL - ^                        | Edit another file N (same as ": e # N")                      |
| 3938 | File editing                                                 |                            gf                            | or] f Edit file with name under cursor                       |
| 3939 | File editing                                                 |                          : pwd                           | Show current directory                                       |
| 3940 | File editing                                                 |                       : cd [path]                        | Change current directory to [path]                           |
| 3941 | File editing                                                 |                          : cd -                          | Return to the previous current directory                     |
| 3942 | File editing                                                 |                        : f [ile]                         | Display current filename and cursor position                 |
| 3943 | File editing                                                 |                     : f [ile] {name}                     | Change current file name to {name}                           |
| 3944 | File editing                                                 |                         : files                          | Display another file list                                    |
| 3945 | Save and Exit                                                |                  : [range] w [rite] [!]                  | Save to the current file                                     |
| 3946 | Save and Exit                                                |                : [range] w [rite] {file}                 | If {file} does not exist, it is saved in {file}.             |
| 3947 | Save and Exit                                                |                : [range] w [rite]! {file}                | Save to {file}. If there is a file overwrite it.             |
| 3948 | Save and Exit                                                |                : [range] w [rite] [!] >>                 | Add to current file                                          |
| 3949 | Save and Exit                                                |             : [range] w [rite] [!] >> {file}             | Add to {file}                                                |
| 3950 | Save and Exit                                                |                : [range] w [rite]! {cmd}                 | Execute {cmd} with [range] line as standard input.           |
| 3951 | Save and Exit                                                |                 : [range] up [date] [!]                  | If it has been changed, overwrite it                         |
| 3952 | Save and Exit                                                |                      : wa [ll] [!]                       | Overwrite and save all changed buffers                       |
| 3953 | Save and Exit                                                |                        : q [uit]                         | If there is no change, the current buffer is ended. If there is no other buffer than help, exit vim. |
| 3954 | Save and Exit                                                |                        : q [uit]!                        | Discard the changes and exit the current buffer. If there is no other buffer than help, exit vim. |
| 3955 | Save and Exit                                                |                        : qa [ll]                         | Exit vim unless changed                                      |
| 3956 | Save and Exit                                                |                        : qa [ll]!                        | Forcibly stop vim even if there is a change                  |
| 3957 | Save and Exit                                                |                           : cq                           | It exits without saving and returns an error code.           |
| 3958 | Save and Exit                                                |                         : wq [!]                         | Save the current file and exit                               |
| 3959 | Save and Exit                                                |                     : wq [!] {file}                      | Save to {file} and exit                                      |
| 3960 | Save and Exit                                                |                   : x [it] [!] [file]                    | ": Wq" and but similar, saved only if you are subjected to any change |
| 3961 | Save and Exit                                                |                            ZZ                            | ": X" with the same                                          |
| 3962 | Save and Exit                                                |                            ZQ                            | ":! Q" the same as the                                       |
| 3963 | Save and Exit                                                |                      : Xa [ll] [!]                       | or: [!] wqall exit and save all changed buffers              |
| 3964 | Save and Exit                                                |                      : St [op] [!]                       | Suspend the vim, start a new shell. Is in the ON 'aw' option, if you do not also specify [!] Save the buffer |
| 3965 | Save and Exit                                                |                          CTRL-Z                          | ": Stop" the same.                                           |
| 3966 | Multiple windows command                                     |                         CTRL-W s                         | or: split divided into two windows                           |
| 3967 | Multiple windows command                                     |                      : Split {file}                      | Split window into two, open the {file} with one              |
| 3968 | Multiple windows command                                     |                     : Vsplit {file}                      | Same as above.The window is a vertical division.             |
| 3969 | Multiple windows command                                     |                     : Vertical {cmd}                     | {Cmd} is such that vertical dividing                         |
| 3970 | Multiple windows command                                     |                    : Sf [ind] {file}                     | Split the window, looking in 'path' the {file}, edit it      |
| 3971 | Multiple windows command                                     |                         CTRL-W]                          | Split window and jump to the tag under the cursor            |
| 3972 | Multiple windows command                                     |                         CTRL-W f                         | Split window and jump to under the cursor file               |
| 3973 | Multiple windows command                                     |                         CTRL-W ^                         | Split window and jump to another file                        |
| 3974 | Multiple windows command                                     |                         CTRL-W n                         | or: new create a new empty window                            |
| 3975 | Multiple windows command                                     |                         CTRL-W q                         | or: q [uit] to exit the editing Close the window             |
| 3976 | Multiple windows command                                     |                         CTRL-W c                         | or: cl [ose] Close the window hidden buffer                  |
| 3977 | Multiple windows command                                     |                         CTRL-W o                         | or: to just the current one window 1 on [ly] screen          |
| 3978 | Multiple windows command                                     |                         CTRL-W j                         | Move the cursor to the bottom of the window                  |
| 3979 | Multiple windows command                                     |                         CTRL-W k                         | Move the cursor into the top window                          |
| 3980 | Multiple windows command                                     |                      CTRL-W CTRL-W                       | Move the cursor to the bottom of the window (wrap)           |
| 3981 | Multiple windows command                                     |                         CTRL-W W                         | Move the cursor to the window of the above (wrap)            |
| 3982 | Multiple windows command                                     |                         CTRL-W t                         | Move the cursor to the top of the window                     |
| 3983 | Multiple windows command                                     |                         CTRL-W b                         | Move the cursor to the window at the bottom                  |
| 3984 | Multiple windows command                                     |                         CTRL-W p                         | Move the cursor to just before the active window of          |
| 3985 | Multiple windows command                                     |                         CTRL-W r                         | To rotate the window on the lower side.                      |
| 3986 | Multiple windows command                                     |                         CTRL-W R                         | To rotate the window on the upper side.                      |
| 3987 | Multiple windows command                                     |                         CTRL-W x                         | Replaced the current window and the next window              |
| 3988 | Multiple windows command                                     |                         CTRL-W =                         | At the same height of all the windows                        |
| 3989 | Multiple windows command                                     |                         CTRL-W -                         | Reduce the height of the current window                      |
| 3990 | Multiple windows command                                     |                         CTRL-W +                         | Increasing the height of the current window                  |
| 3991 | Multiple windows command                                     |                         CTRL-W _                         | To change the height of the current window (default: maximum) |
| 3992 | Buffer management command                                    |                        : Buffers                         | or: files list of all the buffer and the file name           |
| 3993 | Buffer management command                                    |                          : Ball                          | or: sball edit the whole argument / buffer                   |
| 3994 | Buffer management command                                    |                         : Unhide                         | or: Edit the entire buffer of sunhide Loading                |
| 3995 | Buffer management command                                    |                      : Badd {fname}                      | Add file name {fname} to the buffer list                     |
| 3996 | Buffer management command                                    |                    : [!] Bunload [N]                     | [N] No. release the buffer from memory                       |
| 3997 | Buffer management command                                    |                    : [!] Bdelete [N]                     | Remove from the buffer list to open the [N] th buffer        |
| 3998 | Syntax highlighting                                          |                       : Syntax on                        | Start use of syntax highlighting                             |
| 3999 | Syntax highlighting                                          |                       : Syntax off                       | Stop Using syntax highlighting                               |
| 4000 | Syntax highlighting                                          |                     : Syntax [list]                      | To list an item in the current syntax                        |
| 4001 | Syntax highlighting                                          |                      : Syntax clear                      | To delete all of the syntax                                  |
| 4002 | Syntax highlighting                                          |                    : Highlight clear                     | To delete all of the highlights                              |
| 4003 | Syntax highlighting                                          |                      : Filetype on                       | Syntax highlighting to enable the file type of detection is not enabled |
| 4004 | Syntax highlighting                                          |               : Filetype plugin indent on                | To enable the settings and auto-indent to enable file type detection |
| 4005 | Folding command                                              |                 set foldmethod = manual                  | Manually folding                                             |
| 4006 | Folding command                                              |                 set foldmethod = indent                  | Folding in the indent                                        |
| 4007 | Folding command                                              |                  set foldmethod = expr                   | Folding in the 'foldexpr'                                    |
| 4008 | Folding command                                              |                 set foldmethod = syntax                  | Folding in the region of syntax                              |
| 4009 | Folding command                                              |                 set foldmethod = marker                  | Folding in the 'foldmarker'                                  |
| 4010 | Folding command                                              |                       zf {motion}                        | To define the folding manually                               |
| 4011 | Folding command                                              |                      : {Range} fold                      | Folding {range} range of lines                               |
| 4012 | Folding command                                              |                            zd                            | To remove the folding of one under the cursor                |
| 4013 | Folding command                                              |                            zD                            | To remove a folding all under the cursor of                  |
| 4014 | Folding command                                              |                            zo                            | Open one stage folding under the cursor                      |
| 4015 | Folding command                                              |                            zO                            | Open all the stages of folding under the cursor              |
| 4016 | Folding command                                              |                            zc                            | Close one stage folding under the cursor                     |
| 4017 | Folding command                                              |                            zC                            | Close all stages of folding under the cursor                 |
| 4018 | Folding command                                              |                            zm                            | Reduce the 'foldlevel', increasing the number of folding     |
| 4019 | Folding command                                              |                            zM                            | The 'foldlevel' to 0, folding all                            |
| 4020 | Folding command                                              |                            zr                            | Increase the 'foldlevel', reduce the folding                 |
| 4021 | Folding command                                              |                            zR                            | The 'foldlevel' to the maximum, open all                     |
| 4022 | Folding command                                              |                            zn                            | Disable the 'foldenable', without folding                    |
| 4023 | Folding command                                              |                            zN                            | Enable the 'foldenable', folding                             |
| 4024 | Folding command                                              |                            zi                            | To reverse the 'foldenable'                                  |