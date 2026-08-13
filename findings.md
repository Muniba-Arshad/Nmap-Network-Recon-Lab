Nmap Findings

1. Local Host Scan

The local machine was scanned using Nmap.

Target:

127.0.0.x

Observed Ports

Port	    State	  Service
135/tcp	  Open	  MSRPC
445/tcp  	Open  	Microsoft-DS
3306/tcp	Open	  MySQL
443/tcp  	Closed	HTTPS

2. Interpretation

Port 135

TCP port 135 was open and associated with Microsoft RPC services.

Port 445

TCP port 445 was open and associated with Windows networking/SMB-related services.

Port 3306

TCP port 3306 was open and Nmap identified MySQL.

This does not automatically mean that MySQL is vulnerable. An open port only shows that the service is accessible.

Port 443

TCP port 443 was closed.

This means the host was reachable, but no service was accepting connections on that port during the scan.

3. Host Discovery

The local network was checked using:

nmap -sn 192.168.1.0/24

The scan identified multiple responding devices on the authorized local network.

Some devices had identifiable names or manufacturer information, while others were shown as unknown.

4. Main Lessons

* An IP address identifies a host on a network.
* A subnet represents a network range.
* A port represents a network endpoint where a service may listen.
* Open does not mean vulnerable.
* Service/version information helps with further security assessment.
* Host discovery identifies reachable devices.

Security Note

All scans were performed only against systems and networks that I own or have authorization to test.
