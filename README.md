# Web-Enumeration-WebDAV-Lab
Web enumeration and WebDAV misconfiguration assessment performed on Metasploitable2 lab

# Web Enumeration & WebDAV Misconfiguration Lab

## Overview
This mini project demonstrates web application enumeration and WebDAV misconfiguration analysis performed in a controlled lab environment.

All testing was conducted on **Metasploitable2 (local lab)** for learning purposes only.

## Target
- Metasploitable2 (Local Lab)

## Objective
- Discover hidden directories and sensitive endpoints
- Identify WebDAV misconfiguration
- Demonstrate potential impact through controlled interaction

## Tools Used
- DIRB
- Gobuster
- FFUF
- cadaver

## Methodology
1. Performed directory and file enumeration using DIRB, Gobuster, and FFUF
2. Analyzed HTTP response codes to identify existing resources
3. Identified a WebDAV-enabled directory
4. Connected to the WebDAV service using cadaver
5. Verified file upload capability in the lab environment

## Findings
- Multiple hidden directories discovered
- Sensitive endpoints such as phpinfo and phpMyAdmin identified
- WebDAV service allowed file interaction due to misconfiguration

## Impact
If exposed on a real-world server, such misconfiguration could allow:
- Unauthorized file uploads
- Web shell placement
- Website defacement

## Mitigation
- Disable WebDAV if not required
- Enforce proper authentication and authorization
- Restrict access to sensitive directories
- Follow secure server hardening practices

## Disclaimer
This project was performed strictly in a **local lab environment**.  
These techniques should never be used on real systems without proper authorization.

