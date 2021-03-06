### Columnize output of commands

```
$ mount | column –t
$ cat /etc/passwd | column -t -s :
```

### Create a file of certain size

```
$ dd if=/dev/zero of=out.txt bs=1M count=10
```

### `yes(1)` - Output a string repeatedly

Useful to pipe commands that ask for confirmation to

```
$ yes
$ yes whatevah
```

### `script(1)` - Record a terminal session (commands, their output etc.)
Useful for demonstrations

```
$ script foo.txt
$ echo hihi
# other commands bla bla....
# [Ctrl-D] so that the session is written to foo.txt
```

### Change default web browser

From 
https://wiki.debian.org/DefaultWebBrowser#Default_for_foreign_programs_.28system-wide.29

```
$ update-alternatives --config x-www-browser

$ xdg-settings set default-web-browser firefox-esr.desktop
$ xdg-settings get default-web-browser
```
