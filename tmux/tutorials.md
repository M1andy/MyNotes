# Using tutorials

## prefix key

all the shortcut key are prefixed by the `ctrl+b`

basically all the commands that need to determine a session
using `-t <session-number>` or `-t <session-name>`

## Session control

1. create a new session

`tmux new -s <session-name>`

2. detach from a session

shortcut:`ctrl+b d`
command: `tmux detach` 

3. list all session

shortcut:`ctrl+b s`
command: `tmux ls` 

4. attach to a session

`tmux a`
if you want to determine session, use the follow commands.
`tmux attach -t 0` or `tmux attach -t <session-name>`

5. kill a session

command:
```sh
tmux kiss-session -t <session-number>
# or
tmux kiss-session -t <session-name>
```

6. switch to another session

shortcut:`ctrl+b <session-number>`
command:
```sh
tmux switch -t <session-number>
# or
tmux switch -t <session-name> 
```

7. rename a session

shortcut: `ctrl+b $`
command:
```sh
tmux rename-session -t <session-number> <new-name> 
# or
tmux rename-session -t <old-name> <new-name>
```

## Pane control 

1. split pane

shortcut: 
```
# split pane vertically
ctrl+b "
# split pane horizontally
ctrl+b %
# split pane into a new session 
ctrl+b !
```

2. move cursor

shortcut: 
```
# move to another pane
ctrl+b <arrow>
# move to last pane
ctrl+b ;
# move to next pane
ctrl+b o
```

3. other operation

shortcut:
```
# close pane
ctrl+b x
# zoom in or zoom out 
ctrl+b z
# change pane size
ctrl+b ctrl+<arrow>
# show pane number
ctrl+b q
```
