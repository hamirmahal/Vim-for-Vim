# Vim for Vim
Vim for Vim contains my notes on Vim after watching [Lecture 3: Editors (vim) (2020) by Missing Semester](https://www.youtube.com/watch?v=a6Q8Na575qc).

What is the definition of the word "vim"?

A Google search yields the following:

> vim
>
> /vim/
>
> noun INFORMAL
>
> energy; enthusiasm.
>
> "in his youth he was full of vim and vigor"
>
> Origin
> mid 19th century (originally US): perhaps from Latin, accusative of vis ‘energy’.

"Vim" for [Vim, the text editor](https://en.wikipedia.org/wiki/Vim_(text_editor)), therefore, is energy, or enthusiasm, for Vim!

These are the keybindings I have noted so far from watching the aforementioned lecture.

To open Vim, open a Terminal window on MacOS, and type `vim`, or `Vim`, or `VIM`. Capitalization does not seem to matter.

# Modifying Modes
For each of these, we enter the mode on the right by entering the character in parentheses while in the mode on the left.

INSERT MODE (`esc`)-> NORMAL MODE

NORMAL MODE (`:`)-> "COMMAND LINE" MODE

NORMAL MODE (`c`)-> INSERT MODE
- `c` is followed by its argument, which I think must be a movement command. This command deletes in the direction of the movement command.

NORMAL MODE (`cc`)-> INSERT MODE
- This command also deletes the current line if it is nonempty.

NORMAL MODE (`i`)-> INSERT MODE

NORMAL MODE (`o`)-> INSERT MODE
- This command creates a new line below the current one.

NORMAL MODE (`O`)-> INSERT MODE
- This command creates a new line above the current one.

NORMAL MODE (`Ctrl` + `V`)-> VISUAL BLOCK MODE, which selects rectangular blocks of text

NORMAL MODE (`V`)-> VISUAL LINE MODE, which selects lines of text

NORMAL MODE (`v`)-> VISUAL MODE, which selects text highlighted using movement commands

VISUAL MODE (`y`)-> NORMAL MODE
- Entering normal mode from visual mode this way copies all of the text highlighted in visual mode.

# Command Line Mode
`q` quit

`qa` quit all

`q`! force quit

`qa!` force quit all

`sp` opens a new window in the current tab.

`tabnew` opens a new tab.

# Normal Mode
> Normal mode is home, and that's where you should be most of the time.

— <cite>[39:44 mark of Lecture 3: Editors (vim) (2020) by Missing Semester](https://youtu.be/a6Q8Na575qc?t=2384)</cite>

`b` moves the cursor backward by one word.

`d` takes a movement command as an argument, and deletes in the direction of that argument.

`e` moves the cursor to the end of a word.

`f` takes a character as an argument, and moves the cursor to the first character on the current line equal to its argument.

`h` moves left!

`j` moves down!

`k` moves up!

`l` moves right!

`r` takes a character as an argument, and replaces the current character with that argument.

`p` is for paste!

`t` takes a character as an argument, and jumps to the next character on the current line immediately before its argument

`u` undo!

`w` moves the cursor forward by one word.

`x` deletes the character over which the cursor is hovering.

`y` takes a movement command as its argument, and copies text in the direction of its argument.
- For example, `ye` copies to the end of the word.

`F` takes a character as an argument, and moves the cursor to the first character on the current line before its argument, like `f`, above.

`G` moves all the way down.

`H` moves the cursor to the highest line shown on the screen.

`L` moves the cursor to the lowest line shown on the screen.

`M` moves the cursor to the middle line shown on the screen.

`T` takes a character as its argument, and moves the cursor back to the first character in front of its argument on the current line.

`0` moves the cursor to the beginning of a line.

`$` moves the cursor to the end of a line.

`^` moves the cursor to the first nonempty character on a line.

`dd` deletes the current line.

`gg` moves all the way up!

`yy` copies the current line.

`Ctrl` + `D` scrolls down!

`Ctrl` + `R` is redo.

`Ctrl` + `U` scrolls up!

VISUAL MODE

`h` moves left!

`j` moves down!

`k` moves up!

`l` moves right!

`~` flips the cases of the current selection.
- For example, selecting "Visual Studio Code", and pressing `~` while in visual mode results in "vISUAL sTUDIO cODE".

I hope you find these notes helpful!
