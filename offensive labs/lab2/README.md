This lab demonstrates the manual analysis of Application Layer protocols. By stripping away the browser interface and using the telnet client to connect directly to Port 80, I manually constructed raw HTTP/1.1 requests. This exercise focused on understanding the structure of GET requests, the importance of the Host header in virtual hosting, and how to interact with web servers (Nginx) at a low level to retrieve hidden files (flag.html).

Key Skills Demonstrated:

Protocol Analysis: Understanding the raw syntax of HTTP/1.1 (Methods, Headers, Status Codes).

Manual Enumeration: Interacting with listening services without automated tools.

Service Fingerprinting: Identifying server versions (Nginx 1.18.0) via response headers.
