Securing a Networked System with PKI
Project Overview

This project demonstrates the implementation of a secure HTTPS web server using Public Key Infrastructure (PKI) on Kali Linux. The system uses a complete certificate trust chain consisting of a Root Certificate Authority (Root CA), a Subordinate Certificate Authority (AcmeCA), and a Server Certificate to establish secure communication.

The project also includes DNS configuration, Apache HTTPS deployment, firewall hardening, and TLS traffic verification using Wireshark.

Features

✅ Public Key Infrastructure (PKI) Implementation
✅ Root CA and Subordinate CA Configuration
✅ SSL/TLS Certificate Generation and Signing
✅ Apache2 HTTPS Server Deployment
✅ DNS Configuration for Custom Domain
✅ UFW Firewall Security Rules
✅ Secure File Upload Portal
✅ Browser Certificate Validation
✅ TLS Handshake Analysis using Wireshark

Technologies Used
Kali Linux
OpenSSL
Apache2
BIND DNS
UFW Firewall
Wireshark
HTML
SSL/TLS
PKI Architecture
Root CA
   │
   ▼
AcmeCA (Subordinate CA)
   │
   ▼
Server Certificate
   │
   ▼
www.verysecureserver.com
Project Workflow
1. Create Certificate Authorities
Root CA created using OpenSSL
Subordinate CA (AcmeCA) signed by Root CA
2. Configure Apache HTTPS Server
Installed Apache2
Enabled SSL modules
Configured HTTPS virtual host
3. Configure DNS

Mapped the custom domain:

www.verysecureserver.com

to the local server.

4. Configure Firewall

Allowed only required services:

Service	Port
DNS	53
HTTP	80
HTTPS	443
SSH	22
5. Generate CSR and Sign Certificate
Generated server private key
Created Certificate Signing Request (CSR)
Signed the CSR using AcmeCA
6. Install SSL Certificates

Configured Apache to use:

Server Certificate
Private Key
CA Chain
7. Trust Root CA

Imported Root CA into the browser certificate store to establish trust.

8. Verify Secure Communication

Verified HTTPS functionality through:

Browser padlock inspection
Certificate chain validation
Wireshark packet analysis
Secure File Upload Portal

A simple HTTPS-based file upload page was developed to demonstrate secure communication between client and server.

Features
HTTPS Protected
TLS Encryption
Certificate Validation
Secure File Upload Interface
TLS Verification with Wireshark

Captured and analyzed HTTPS traffic using Wireshark.

Observed:

TCP Three-Way Handshake
Client Hello
Server Hello
Certificate Exchange
Change Cipher Spec
Encrypted Application Data

This confirmed that all communication was protected using TLS encryption.

Project Demonstration Video

🎥 Watch the complete project demonstration:

Google Drive Link

https://drive.google.com/file/d/1I4BwN4xtv9JJbqAU8gtxUe0hyJ95ryi_/view?usp=sharing

Screenshots

Add screenshots in a folder named:

screenshots/

Suggested screenshots:

Certificate Chain
Browser HTTPS Verification
Secure Upload Portal
Wireshark TLS Handshake
Apache SSL Configuration
Learning Outcomes
Understanding Public Key Infrastructure (PKI)
Certificate Authority Hierarchies
SSL/TLS Deployment
Apache HTTPS Configuration
DNS Management
Network Security Monitoring
Packet Analysis with Wireshark
Team Members
Name	ID
MD Arham Jawed Akib	2022-3-60-004
Jannatul Ferdaus Oishi	2022-3-60-216
Mahin Ahmed Meghla	2022-3-60-152
Course Information

Course: CSE487 – Network Security
Semester: Summer 2025
Department: Computer Science & Engineering
University: East West University

License

This project was developed for academic and educational purposes.
