This was my first ever lab related to CyberSecurity from TCM Security, This script is a command-line port scanner designed to probe a target server for open ports. It utilizes Python's low-level networking interface to establish TCP connections, effectively simulating the initial steps of a network vulnerability assessment.

Key Features:

Target Resolution: Automatically converts hostnames to IPv4 addresses using socket.gethostbyname.

TCP Connect Scan: Uses SOCK_STREAM sockets to attempt full 3-way handshakes, accurately verifying if a port is open.

Error Handling: Includes robust exception handling for Keyboard Interrupts (Ctrl+C) and DNS resolution errors (socket.gaierror), ensuring the script exits gracefully during operations.

Performance: Implements a strict timeout (socket.setdefaulttimeout) to prevent hanging on filtered or non-responsive ports.

Usage:

Bash
python3 scanner.py <target_ip>
