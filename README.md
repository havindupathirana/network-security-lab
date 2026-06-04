# Network Security Lab

## Overview

This project demonstrates the implementation of a secure Linux server environment using Ubuntu and Kali Linux.

Key technologies:

- OpenSSH
- SSH Key Authentication
- Multi-Factor Authentication (MFA)
- Cowrie Honeypot
- iptables Firewall

## Architecture

Kali Linux
    |
 SSH 2233
    |
Ubuntu Server
 ├── OpenSSH + MFA
 ├── Cowrie Honeypot
 └── iptables Firewall

## Features

### SSH Hardening
- Root login disabled
- Password authentication disabled
- Key-based authentication enabled
- Custom SSH port

### Multi-Factor Authentication
- Google Authenticator integration
- OTP verification for SSH access

### Cowrie Honeypot
- SSH and Telnet emulation
- Attack logging and monitoring

### Firewall Protection
- Default deny policy
- Traffic logging
- Port redirection to honeypot

## Lessons Learned

- SSH security requires multiple layers of protection.
- MFA significantly reduces account compromise risk.
- Honeypots provide visibility into attacker behaviour.
- Firewalls should follow a default-deny approach.

## Technologies Used

- Ubuntu Linux
- Kali Linux
- OpenSSH
- Cowrie
- Google Authenticator PAM
- iptables
