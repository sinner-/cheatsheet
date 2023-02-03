# socat Cheatsheet

* Listen on a port and execute a command when connection established
  * `socat -v -s -d -d tcp-listen:80,reuseaddr,fork,bind=192.168.1.1 exec:"echo ----"` (netcat doesn't show the incoming IP)
