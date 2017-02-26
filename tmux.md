# tmux Cheatsheet

* New session:
  * `tmux new -s <SESSION_NAME>`
* Attach to existing session:
  * `tmux attach -t <SESSION_NAME>`
* Attach to existing session and detach all other sessions:
  * `tmux attach -dt <SESSION_NAME>`
* New window:
  * `Ctrl-b + c`
* Switch to next window:
  * `Ctrl-b + n`
* Switch to window (0<=WINDOW_NUMBER<=9):
  * `Ctrl-b + <WINDOW_NUMBER>`
* Show window index:
  * `Ctrl-b + w`
* Rename window:
  * `Ctrl-b + ,`
* Split window vertically:
  * `Ctrl-b + %`
* Split window horizontally:
  * `Ctrl-b + "`
* Switch between split panes:
  * `Ctrl-b + <ARROW_KEY>`
* Resize split panes:
  * `Hold Ctrl-b + <ARROW_KEY>`
* Enter copy mode (scroll, search, copy/paste):
  * `Ctrl-b + [`
* Copy mode commands:
  * Copy:
    * Navigate to start of text to copy.
    * `Ctrl + Space`
    * Select region to copy.
    * `Alt + w`
  * Paste selection:
    * `Ctrl-b + ]`
  * Save selection to file:
    * `Ctrl-b + :`
    * `save-buffer /tmp/out_file`
  * Search up:
    * `Ctrl - r`
  * Search down:
    * `Ctrl - s`
* Save buffer:
  * `Ctrl-b + :`
  * `capture-pane -S -<NUMBER_OF_LINES_TO_SAVE>`
  * `Ctrl-b + :`
  * `save-buffer /tmp/out_file`
