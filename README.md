# VIM (VI Improved)
This file holds record about my findings to learn how to use VIM editor. Very useful when you have access to a server, but can't download any file, or can't use any modern editors(e.g - VSCode) there.

## VIM Modes
- Normal Mode (by default, can apply different commands)
- Insert Mode (press i on keyboard to switch to, or a for append, used to start editing)
- Visual Mode (press esc to switch to normal mode, then press v, helps to select, copy, delete etc. operations)

### Commands for vim editor:
--------------------------
1. Find the occurance of a word - esc > /word, e.g - to find the word 'dev', press esc and type /dev, the word should be exact match. To navigate - 
        n - next occurence
        N - previous occurance
        # - previous token occurance
        + - next token occurance
2. :set number - show line numbers
3. :set relativenumber - show number relative to current cursor position, e.g - 2 lines up will be 2
4. :colorscheme [name of the scheme] - press tab to find different color scheme
5. :set tabstop=4 - Tabs width set to 4 spaces
6. :set autoindent - Auto indentatation
7. :set mouse=a - Activate the mouse
8. :set mouse="" - Deactivate Mouse
