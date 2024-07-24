# VIM (VI Improved)

This file holds record about my findings to learn how to use VIM editor. Very useful when you have access to a server, but can't download any file, or can't use any modern editors(e.g - VSCode) there.

## VIM Modes

- Normal Mode (by default, can apply different commands)
- Insert Mode (press i on keyboard to switch to, or a for append, used to start editing)
- Visual Mode (press esc to switch to normal mode, then press v, helps to select, copy, delete etc. operations)
- Replace Mode (esc > R), this replaces the content right after the cursor

### Inserting, Appending, Adding lines

- i - get into insert mode
- a - append, adds at the end
- I - insert before a line
- A - append after a line
- o - new line below, and insert mode
- O - new line above, and insert mode


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

- hjkl - left, bottom, up, right navigation
- w - jump one word  
- b - jump one word backward  
- 20w - jump 20 words  
- 14b - jump 14 words back  
- 8k - jump 8 lines on top
- % - jump from opening to closing of a bracket
- gg - beginning of a file
- G - end of a file
- 17G - go to line number 17
- :17 - go to line number 17
- $ - end of a line
- 0 - beginning of a line

### Undo/Redo

- u - undo  
- Ctrl + R - redo

- 5u - undo the last 5 operations  
- 4Ctrl + R - redo the last 4 operations  

### Replacing, Changing, Deleting

- r - replace a letter
- R - replace mode, overrides the content starting from the cursor to the next
- cw - replace a word, w is for word, will work from the cursor  
- c7w - replace 7 words  
- C - delete the rest of the line and go to insert mode  
- D - delete without going to insert mode  
- D2w - delete the next 2 words  
- cc - replace the whole line  
- 9cc - replace the next 9 lines
- dd - delete the whole line
- 4dd - delete the next 4 lines
- ciw - change inner word, i.e - selecting the whole word by putting the cursor anywhere in the word  
- diw - delete inner word
- c% - change everything from this bracket to that bracket
- ggdG - delete whole file, gg for going to top, d to delete everything up to end of file(G)

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

### Repeat

- . - press dot to repeat the last operation, e.g - pasting a content in the file or anything.

### Copy, Paste, Select

- v - visual mode
- V - visual line, select the line where the cursor is
- Ctrl + v - visual block, select blocks manually by navigating top bottom sidewise etc.  

### After selection

- d - delete
- c - change
- y - yanking(copy)
- p - paste after
- P - paste before
- yy - yank/copy whole line
- 5yy - copy the next 5 lines
- 9p - paste 9 lines
- y5w - yank 5 words
- yiw - yank inner word
- yi) - copy everything up to this bracket  

### Indentation and Shifting

- \> shift right the selected block
- \< - shift left the selected block
- = - indent the selected block
- \>> & << - Shift the line where cursor is
- == - Indent the line where cursor is
- gg=G - Indent the whole file, gg for navigating to beginning of the file, then indent (=) up to G which means end of file

### Others

zz - center selected line, even if the cursor is in the end of file, that will show centered on the screen.
