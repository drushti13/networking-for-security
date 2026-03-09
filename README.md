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

| Layer Number | Layer Name            | Main Function                                             | Example Protocols and Standards            |
|--------------|-----------------------|-----------------------------------------------------------|--------------------------------------------|
| Layer 7      | Application Layer     | Providing services and interfaces to applications         | HTTP, FTP, DNS, POP3, SMTP, IMAP           |
| Layer 6      | Presentation Layer    | Data encoding, encryption, and compression                | Unicode, MIME, JPEG, PNG, MPEG             |
| Layer 5      | Session Layer         | Establishing, maintaining, and synchronising sessions     | NFS, RPC                                   |
| Layer 4      | Transport Layer       | End-to-end communication and data segmentation            | UDP, TCP                                   |
| Layer 3      | Network Layer         | Logical addressing and routing between networks           | IP, ICMP, IPSec                            |
| Layer 2      | Data Link Layer       | Reliable data transfer between adjacent nodes             | Ethernet (802.3), WiFi (802.11)            |
| Layer 1      | Physical Layer        | Physical data transmission media                          | Electrical, optical, and wireless signals  |

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

## Common Port

| Protocol | Transport Protocol | Default Port Number |
|---------|-------------------|--------------------|
| TELNET  | TCP               | 23                 |
| DNS     | UDP or TCP        | 53                 |
| HTTP    | TCP               | 80                 |
| HTTPS   | TCP               | 443                |
| FTP     | TCP               | 21                 |
| SMTP /SMTPS    | TCP               | 25 /465 and 587                |
| POP3 / POP3S   | TCP               | 110 /995             |
| IMAP /IMAPS    | TCP               | 143 / 993               |

## Network Protocols

| Protocol | Full Form | Main Purpose | Typical Use Case |
|----------|-----------|--------------|------------------|
| **ARP** | Address Resolution Protocol | Maps an IP address to a MAC address within a local network. | Used when a device needs the MAC address of another device on the same LAN. |
| **DHCP** | Dynamic Host Configuration Protocol | Automatically assigns IP addresses and other network settings to devices. | When a device connects to a network and receives an IP address automatically. |
| **ICMP** | Internet Control Message Protocol | Used for network diagnostics and error reporting. | Commands like `ping` and `traceroute` rely on ICMP. |
| **NAT** | Network Address Translation | Translates private IP addresses to a public IP address for internet communication. | Home routers allowing multiple devices to share one internet connection. |
| **FTP** | File Transfer Protocol | Transfers files between a client and a server over a network. | Uploading or downloading files from a server. |
| **SMTP** | Simple Mail Transfer Protocol | Sends and relays outgoing email between mail servers. | Used when sending an email. |
| **POP3** | Post Office Protocol Version 3 | Retrieves emails from a mail server and typically downloads them to a client device. | Email clients downloading messages from a server. |
| **IMAP** | Internet Message Access Protocol | Retrieves and manages email directly on the mail server without downloading all messages. | Synchronizing email across multiple devices. |
| **WHOIS** | Whois Protocol | Queries databases to retrieve information about domain name registrations. | Checking domain ownership and registration details. |
