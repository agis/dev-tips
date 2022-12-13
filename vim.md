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

------------------

MOVING
--------
^ – jump to the first (non-blank) character of the line
[[ (or ]]) - jump to beginning of enclosing function

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
