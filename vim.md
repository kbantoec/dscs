# VIM 

## Modes
Vim has 3 primary modes:
1. Normal

### Normal mode
Use `h` (left), `j` (down), `k` (up), and `l` (right) to navigate.

Shortcut: Type `5k` to go 5 lines up, for example.

Type
* `w` to go at the beginning of the next word
* `b`to go at the beginning of the previous word
* `e` to move at the end of the word
* `0` to move at the start of the line
* `$` to move at the end of the line
* `gg` to move at the beginning of the document
* `shift + g` to move at the end of the document

| Command | Description |
| - | - |
`:w`| Save
`:q`| Quit
`:wq` | Save then quit
`u` | Undo
`ctrl + r`| Redo
`i`| Turn into insert mode
`v` | Visual mode (used for selection)
`y` | Copy (or "yank" in Vim language)
`p` | Paste
`dd`| Delete the entire current line
`d<number>w`| Delete N words
`<number><h/j/k/l>` | Go `<left/down/up|right>` N lines
 `vi ~/.vimrc` |  Open this file to save your settings

## Example of a .vimrc file
```vim
set number
set relativenumber
set tabstop=4
set shiftwidth=4
set autoindent
set mouse=1
coloscheme slate
```
