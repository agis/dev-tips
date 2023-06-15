### Format the selected block according to column rules (word-wrap)

```
select block + gq
```

### Zoom a particular window and restore it:

Zoom in: `c-w-|`
Zoom out: `c-w-=`

### Opening fzf result in split windows

- Hitting Ctrl-x will open the file under the cursor as a horizontal split.
- Hitting Ctrl-v will alternatively open that file as a vertical split.
- Hitting Ctrl-t will alternatively open that file in a new tab.

------------------

MOVING
--------
^ – jump to the first (non-blank) character of the line

[[ and ]] - jump to beginning of enclosing function
{{ and }} - jump to next paragraph

'. - jump to last edit
`` - jump back to where you jumped from

ctrl-u and ctrl-d - scroll page up/down
ctrl-y and ctrl-e - move up/down 1 line without moving cursor

2f, - jump to the second next comma character
; - move to the next character (after using f/t)
, - move to the previous character (after using f/t)


EDITING
--------
gj – merge the line below to the current one with no space in between them
ciw - change word under cursor
cip - change paragraph under cursor


SEARCHING
----------
# – jump to previous instance of the current word
?pattern – search backward for the specified pattern
F - like f, but backwards (find next character)
T - like t, but backwards (find next character)

COMMANDS
--------
:sav – save the file under a new name and continue editing the new copy
:w !sudo tee % – write out the file using sudo and tee command

AUTOCOMPLETION
--------------
In Insert mode, <C-x><C-f> to autocomplete files. <C-x><C-k> to autocomplete
based on a dictionary.
