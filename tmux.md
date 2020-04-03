# Tmux Help

### Tmux Settings
- Config file ~.tmux.conf

### Commands in tmux
- CTRL + B -> Tmux commands
- CTRL + B + I -> Install plugins
- CTRL + B + U -> Update plugins
- ? -> Help -> Enter for leave help
- D (+ ENTER) -> detach
- n -> switch between windows
- & -> close activ windows
- 1 etc. -> switch between windows \<number>
- c -> create new window
- o -> switch between panes
- x -> kill pane
- , \<name> -> rename window
- :swap-window -s \<number1> -t \<number2> -> swap window \<number1> with window \<number2>
- [ -> copy mode (vim movement keys for "scrolling") 
- Space (+ vim movement keys) -> select text
- Enter -> stop selecting
- ] -> paste

### Tmux related commands for bash
- tmux ls -> list sessions
- tmux a -> attach
- tmux a -t \<name> -> attach to sesstion with name
- tmux kill-session -t \<name> -> kill session with name
- tmux kill-server -> kill all tmux sessions

### Tmux Sessions
- CTRL + B + CTRL + s -> Save tmux session
- CTRL + B + CTRL + r -> Restore tmux session