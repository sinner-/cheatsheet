# dnf Cheatsheet

* Write LiveCD ISO to USB:
  * `dd if=.iso of=/dev/sdb bs=1M oflag=sync`
* View progress of dd (GNU coreutils 8.24+)
  * `dd if=/dev/zero of=/dev/null count=1000 status=progress`
