# SilentPass
A lightweight C# reverse shell for authorized penetration testing and red team operations. Includes AMSI bypass capabilities and process injection techniques for security research purposes. Capable of bypassing Bitdefender antivirus and delivering a full interactive shell back to your Netcat listener.

Features
Bypasses Bitdefender antivirus detection
Delivers interactive PowerShell shell back to Netcat listener
AMSI bypass integration for PowerShell evasion
Hidden window execution (no console popup)
TCP reverse shell communication
Stream-based I/O redirection
Multi-threaded output handling
Execution policy bypass

How It Works
SilentPass establishes a TCP connection from the target machine to your listener, spawns a hidden PowerShell process with AMSI disabled, and routes all console input/output through the network socket. This gives you remote command execution as if you were sitting at the target's keyboard.

Tested Against
Bitdefender Total Security (bypassed)
