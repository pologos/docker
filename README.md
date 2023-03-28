# docker

How it works?

the system is working on demand with local environment + external api to add some new features

poloshell (port:8022) --[command]--> (port:80) apicontext --[text2botreck]--> botreck plugin on browser

poloshell (port:8022) --[command]--> apicontext --[text2apidsl]--> (port:22) shell with native commands





## Tech stack

+ fedora os 
+ shell:
  + bash (22) - admin terminal
  + fish (2222) - user terminal
  + poloshell (8022) - customer web terminal to write commands
+ apicontext: convert the commands from poloshell to botreck on browser
+ browser: chromium 
+ browser plugins: botreck 
+ remotedekstop
+ keepass - local passwords


### List All Open Ports

Before opening a port on Linux, you must check the list of all open ports, and choose an ephemeral port to open that is not on that list.

Use the netstat command to list all open ports, including TCP and UDP, which are the most common protocols for packet transmission in the network layer.

    netstat -lntu

This will print:

    all listening sockets (-l)
    the port number (-n)
    TCP ports (-t)
    UDP ports (-u)


Verify that you are receiving consistent outputs using the ss command to list listening sockets with an open port:

    ss -lntu



Ensure that port 4000 is not used using the netstat command:

    netstat -na | grep :4000

Or the ss command:

    ss -na | grep :4000



## Common ports number and services

FTP - 21

So, port 21 is used for FTP (File Transfer Protocol). The major use case of FTP is to exchange files between client and server.

By default, FTP does not include encryption for files being sent over the established connections and is often considered a risk.
SSH - 22

SSH (Secure Shell) is widely used by advanced users or system admins to access remote computers. But you can also use SSH for the transmission of data over the network.

SSH uses cryptographic techniques which ensure that the connection between a remote server and your computer is encrypted.
TELNET - 23

TELNET stands for TErminaL NETwork. It is used to connect computers over the internet or local computers and provides bidirectional interactive text-oriented communication.

TELNET does not provide any kind of encryption, and this is the major reason why it is only used to connect local machines.
SMTP - 25

Simple Mail Transfer Protocol (SMTP) is used to send messages, but can not receive them because it can't queue messages at the receiver point.

So it is often paired with other protocols such as POP3 or IMAP for receiving messages.
DNS - 53

This is one of my personal favorites, as it turns the domain name into an IP address. So you may write any keyword in your search bar and don't have to remember the IP address for each site.

[Common Networking Port Numbers in Linux](https://linuxhandbook.com/common-ports/)

> You can also refer to the given table that includes the most common ports with port no. and the protocol it uses:
> 
> | Port No | Port | Protocol |
> | --- | --- | --- |
> | 21 | FTP | TCP |
> | 22 | SSH | TCP |
> | 23 | TELNET | TCP |
> | 25 | SMTP | TCP |
> | 53 | DNS | TCP, UDP |
> | 67,68 | DHCP | UDP |
> | 80 | HTTP | TCP |
> | 110 | POP3 | TCP |
> | 111 | Portmapper | TCP, UDP |
> | 123 | NTP | UDP |
> | 137 | NetBIOS | TCP, UDP |
> | 143 | IMAP | TCP, UDP |
> | 161,162 | SNMP | UDP |
> | 443 | HTTPS | TCP |

### Automatisation

over browser + keepass passworts + shell commands


## Fedora os

OS on docker with option to connect throughr RDP
fast and is working as default with remote desktop to use it on windows environment


## EXAMPLE:

selektory CSS, generuj 


