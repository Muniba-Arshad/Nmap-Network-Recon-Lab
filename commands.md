Nmap Commands

This file contains the Nmap commands I practiced during the lab and explains when each command is useful.

1. Check Network Information

ipconfig

What it does

Shows the computer’s network configuration.

It can show:

* IPv4 address
* Subnet mask
* Default gateway

Why I used it

I used it to identify my local IPv4 address and understand my local network range.


2. Basic Nmap Scan

nmap TARGET

What it does

Performs a basic scan of the target and checks commonly used ports.

When to use it

Use this when you want a basic view of which ports are open or closed on an authorized target.

Example

nmap 192.168.1.x


3. Service and Version Detection

nmap -sV TARGET

What it does

Attempts to identify the services and software versions running on open ports.

When to use it

Use this when you already know that ports are open and want more information about the services behind them.

Example

nmap -sV 192.168.1.x



4. Scan a Specific Port

nmap -p PORT TARGET

What it does

Scans only the port that you specify.

When to use it

Use this when you want to investigate one particular port instead of scanning many ports.

Example

nmap -p 3306 127.0.0.x

Port 3306 is commonly associated with MySQL.


5. Scan Multiple Specific Ports

nmap -p 22,80,443 TARGET

What it does

Scans only the specified ports.

When to use it

Useful when you want to check a small group of known ports.



6. Host Discovery

nmap -sn NETWORK

What it does

Discovers hosts that respond on the specified network without performing a normal port scan.

When to use it

Use this when you want to know which devices are reachable on an authorized local network.

Example

nmap -sn 192.168.1.0/24


Security Reminder

Nmap should only be used against systems and networks that you own or have explicit permission to test.
