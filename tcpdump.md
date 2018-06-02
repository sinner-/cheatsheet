# tcpdump Cheatsheet

* Listen on an interface:
  * `tcpdump -i <interface name>`
* Don't perform DNS lookups on addresses:
  * `tcpdump -n`
  * `tcpdump -nn` (don't convert protocol/port to names as well)
* Listen on a port:
  * `tcpdump tcp port 22`
* Listen on multiple ports:
  * `tcpdump tcp port 22 or tcp port 23`
* Listen for packets from a source address:
  * `tcpdump src <address>`
* Listen for packets to a destination address:
  * `tcpdump dst <address>`
* Filter a protocol (e.g. ARP):
  * `tcpdump \!arp`
* Write PCAP file instead of parsing and printing:
  * `tcpdump -w file.pcap`
  * `tcpdump -w -` (write to stdout)
  * `tcpdump -wU` (write without buffering)
* Read from PCAP file:
  * `tcpdump -r <filename>`
  * `tcpdump -r -` (read from stdin)
* Most verbose output:
  * `tcpdump -vvv
* Print packet dump in hex:
  * `tcpdump -xx`
* Print packet dump in ASCII:
  * `tcpdump -XX`
* Put WiFi into monitor mode:
  * `tcpdump --monitor-mode`
