# Vim - cheat sheet

## Table of contents
- [Working with file](#working-with-file)
- [Searching](#searching)
- [Moving](#moving)
   * [Moving within the line](#moving-within-the-line)
   * [Moving by word](#moving-by-word)
   * [Moving by sentence or paragraph](#moving-by-sentence-or-paragraph)
   * [Moving within the screen](#moving-within-the-screen)
- [Modifying](#modifying)
   * [Undo](#undo)
   * [Redo](#redo)
   * [Repeat](#repeat)
   * [Delete](#delete)
- [Copy and Paste](#copy-and-paste)
- [Resources](#resources)

## Working with file
|Command|Description|
|-------|-----------|
```vi file``` | Open your file in
```:w```| Write your changes to the file
```:q!```| Quit without saving your changes
```:wq```, ```ZZ``` | Write your changes and exit
```:saveas ~/some/path/```|  Save your file to that location

## Searching
|Command|Description|
|-------|-----------|
```/pattern```, ```?pattern```| Search for string
```t```|  Jump up to a character
```f```|  Jump onto a character
```*```|  Search for other instances of the word under your cursor
```n``` | Go to the next instance when you've searched for a string
```N``` | Go to the previous instance when you've searched for a string
```;``` | Go to the next instance when you've jumped to a character
```,``` | Go to the previous instance when you've jumped to a character

## Moving
|Command|Description|
|-------|-----------|
```j``` | Move down one line
```k``` | Move up one line
```h``` | Move left one character
```l``` | Move right one character

### Moving within the line
|Command|Description|
|-------|-----------|
```0``` | Move to the beginning of the line
```$``` | Move to the end of the line
```^``` | Move to the first non-blank character in the line
```t<one>``` | Jump to right before the next tag
```f<one>``` | Jump and land on the next tag
### Moving by word
|Command|Description|
|-------|-----------|
```w``` | Move forward one word
```W``` | Move forward one big word
```b``` | Move back one word
```B``` | Move back one big word
```e``` | Move to the end of your word
### Moving by sentence or paragraph
|Command|Description|
|-------|-----------|
```)```, ```(``` | Move forward one sentence
```}```, ```{``` | Move forward one paragraph

### Moving within the screen
|Command|Description|
|-------|-----------|
```H``` | Move to the top of the screen
```M``` | Move to the middle of the screen
```L``` | Move to the bottom of the screen
```gg``` | Go to the top of the file
```G``` | Go to the bottom of the file
```^U``` | Move up half a screen
```^D``` | Move down half a screen
```^F``` | Page down
```^B``` | Page up
```:$lineNumber``` | Move to a given line number
```^E``` | Scroll up one line
```^Y``` | Scroll down one line

## Modifying
|Command|Description|
|-------|-----------|
```i``` | Insert before the cursor
```I``` | Insert at the beginning of the line
```a``` | Append after the cursor
```A``` | Append at the end of the line
```o``` | Open a new line below the current one
```O``` | Open a new line above the current one
```r``` | Replace the one character under your cursor
```R``` | Replace the character under your cursor, but just keep typing afterwards
```cm``` | Change whatever you define as a movement, e.g. a word, or a sentence, or a paragraph.
```C``` | Change the current line from where you're at
```ct?``` | Change change up to the question mark
```s``` | Substitute from where you are to the next command (noun)
```S``` | Substitute the entire current line

### Undo
|Command|Description|
|-------|-----------|
```u``` | Undo your last action

### Redo
|Command|Description|
|-------|-----------|
```Ctrl+r```, ```Cmd+r``` | Redo the last action

### Repeat
|Command|Description|
|-------|-----------|
```.``` | Repeat the last action

### Delete
|Command|Description|
|-------|-----------|
```x``` | Exterminate (delete) the character under the cursor
```X``` | Exterminate (delete) the character before the cursor
```dm``` | Delete whatever you define as a movement, e.g. a word, or a sentence, or a paragraph.
```dd``` | Delete the current line
```dt.``` | Delete delete from where you are to the period
```D``` | Delete to the end of the line
```J``` | Join the current line with the next one (delete what's between)

## Copy and Paste
|Command|Description|
|-------|-----------|
```y``` | Yank (copy) from where you are to the next command (noun)
```yy``` | A shortcut for copying the current line
```p``` | Paste the copied (or deleted) text after the current cursor position
```P``` | Paste the copied (or deleted) text before the current cursor position

## Resources
[Learn vim For the Last Time: A Tutorial and Primer](https://danielmiessler.com/study/vim/)
[OpenVim](https://www.openvim.com/)
[Vim adventures](https://vim-adventures.com/)
[Vim genius](http://www.vimgenius.com/)
[Vim Valley](https://vimvalley.com/)