# gpg Cheatsheet

* Generate a new private/public keypair:
  * `gpg --gen-key`
* Export ASCII armoured public key:
  * `gpg --armor --output <ID>`
* Import a public key:
  * `gpg --import keyfile.gpg`
* Encrypt file for recipient with ASCII armouring:
  * `gpg --encrypt --armor --recipient <ID> filetobeencrypted.txt`
* Encrypt content from prompt with ASCII armouring:
  * `gpg --encrypt --armor --recipient <ID>`
  * Type message.
  * `Ctrl-D` to end message.
* Decrypt a file:
  * `gpg --decrypt filetobedecrypted.gpg --output file.txt`
