# SSH Cheatsheet

* Exit a hung SSH session:
  * `Enter + ~ + .`
* Establish SSH tunnel:
  * `ssh <SSH server username>@<SSH server IP> -L 127.0.0.1:9999:<REMOTE HOST IP>:<REMOTE HOST PORT> -N`
