# postfix Cheatsheet

* List queue contents:
  * `postqueue -p`
* Delete message from queue:
  * `postsuper -d <MESSAGE ID>`
* Delete all deferred messages from queue:
  * `postsuper -d deferred`
* Force deliver all messages stuck in queue:
  * `postqueue -f`

