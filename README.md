Nmap Network Reconnaissance Lab

Project Overview

This project documents my practical learning of Nmap for basic network reconnaissance and enumeration in an authorized local lab environment.

Purpose

The purpose of this project was to understand how Nmap can be used to:

* Discover active hosts
* Scan network ports
* Identify services
* Detect service versions
* Understand basic network exposure

Tools Used

* Nmap
* Nmap Zenmap GUI
* Windows
* Command Prompt

Skills Practiced

* Network reconnaissance
* Host discovery
* Port scanning
* Service detection
* Version detection
* Basic network enumeration
* Understanding port states

Lab Environment

* Operating System: Windows
* Network: Authorized local network
* Target: Own device and authorized local network

Key Concepts Learned

Open Port

An open port means that a service is listening and accepting network connections on that port.

Closed Port

A closed port means that the host is reachable, but no service is currently accepting connections on that port.

Filtered Port

A filtered port means that Nmap cannot determine whether the port is open because a firewall or network control is interfering with the scan.

Important Security Concept

An open port does not automatically mean that a system is vulnerable.

An open port means that a service is accessible. Further investigation is required to determine whether the service has a security weakness.

Example Finding

During the lab, Nmap identified:

3306/tcp open mysql

This means TCP port 3306 was open and Nmap identified a MySQL service.

What I Learned

* How to identify a local IPv4 address
* How subnet masks define a network range
* How /24 represents a common IPv4 subnet
* How to discover active hosts
* How to scan ports
* How to identify services and versions
* The difference between open, closed, and filtered ports
* Why an open port does not automatically mean a vulnerability

Security Note

All scanning activities were performed only against systems and networks that I own or have authorization to test.

Project Status

Completed — Basic Nmap Network Reconnaissance Lab
