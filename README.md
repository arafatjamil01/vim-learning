# VIM (VI Improved)

This file holds record about my findings to learn how to use VIM editor. Very useful when you have access to a server, but can't download any file, or can't use any modern editors(e.g - VSCode) there.

## VIM Modes

- Normal Mode (by default, can apply different commands)
- Insert Mode (press i on keyboard to switch to, or a for append, used to start editing)
- Visual Mode (press esc to switch to normal mode, then press v, helps to select, copy, delete etc. operations)
- Replace Mode (esc > R)

### Commands for vim editor

1. Find a specific word - esc > /word, e.g - to find the word 'dev', press esc and type /dev, the word should be exact match. To navigate -
        n - next
        N - previous
        # - previous token
        + - next token
2. :set number - show line numbers
3. :set relativenumber - show number relative to current cursor position, e.g - 2 lines up will be 2
4. :colorscheme [name of the scheme] - press tab to find different color scheme
5. :set tabstop=4 - Tabs width set to 4 spaces
6. :set autoindent - Auto indentation
7. :set mouse=a - Activate the mouse
8. :set mouse="" - Deactivate Mouse

### Navigation

w - jump one word
b - jump one word backward
20w - jump 20 words
14b - jump 14 words back

### Undo/Redo

- u - undo  
- Ctrl + R - redo

- 5u - undo the last 5 operations  
- 4Ctrl + R - redo the last 4 operations  

### Replacing, Changing, Deleting

- r - replace  
- R - replace mode  
- cw - replace a word, w is for word, will work from the cursor  
- c7w - replace 7 words  
- C - delete the rest of the line and go to insert mode  
- D - delete without going to insert mode  
- D2w - delete the next 2 words  
- cc - replace the whole line  
- dd - delete the whole line
- ciw - change inner word, i.e - selecting the whole word by putting the cursor anywhere in the word  
- diw - delete inner word
- c% - change everything from this bracket to that bracket

#### For brackets (useful when programming)

- ci) - change inner content until )  
- ci(  
- ci]  
- ci[  
- ci{  
- ci}  

#### Replace a word in a sentence

- :s/old/new/g, e.g - replace 'dev' with 'ops' in one line - :s/dev/ops/g  
- :%s/old/new/g - replace everywhere
