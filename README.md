# Networking Basics for Cybersecurity

Understanding networking is essential for cybersecurity because most attacks and defenses occur over networks.

This repository contains notes on core networking concepts used in security analysis and penetration testing.

## OSI Model

The OSI model has seven layers:

1. Physical (raw bits)
2. Data Link (MAC address)
3. Network  (IP address)
4. Transport (Port numbers)
5. Session
6. Presentation
7. Application

Each layer handles specific functions in network communication.


Layer Number	   Layer Name	               Main Function	                                         Example Protocols and Standards
Layer 7       	 Application layer	       Providing services and interfaces to applications	        HTTP, FTP, DNS, POP3, SMTP, IMAP
Layer 6	         Presentation layer	        Data encoding, encryption, and compression	           Unicode, MIME, JPEG, PNG, MPEG
Layer 5	         Session layer	               Establishing, maintaining, and synchronising sessions	NFS, RPC
Layer 4	Transport layer	End-to-end communication and data segmentation	UDP, TCP
Layer 3	Network layer	Logical addressing and routing between networks	IP, ICMP, IPSec
Layer 2	Data link layer	Reliable data transfer between adjacent nodes	Ethernet (802.3), WiFi (802.11)
Layer 1	Physical layer	Physical data transmission media	Electrical, optical, and wireless signals

## TCP vs UDP

TCP

- Connection oriented
- Reliable
- Ensures packet delivery
- Used for HTTP, SSH, FTP

UDP

- Connectionless
- Faster but less reliable
- Used for DNS and streaming


## DNS

DNS (Domain Name System) converts domain names into IP addresses.

Example:

Domain:
google.com

Resolved IP:
142.250.x.x

Tools used for DNS lookup:

- nslookup
- dig


## HTTP vs HTTPS

HTTP

- HyperText Transfer Protocol
- Data transmitted in plaintext
- Default port: 80

HTTPS

- Secure HTTP
- Uses encryption via TLS
- Default port: 443

## Common Ports

21 - FTP  
22 - SSH  
23 - Telnet  
25 - SMTP  
53 - DNS  
80 - HTTP  
443 - HTTPS  

These ports are commonly scanned during network reconnaissance.
