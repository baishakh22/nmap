# Version Scan

* Ports are not always what they appear to be. Like port 22 is usually for the SSH and nmap will assume that. 
* "-sV" enables version scanning to determine the actual services
* Also note that time difference from a regular scan to a version scan (14 v 21 seconds for scanning a vm)
* nmap accomplishes this by
    - Listening for 5 seconds for a banner (null probe)
    - UDP / TCP probe
    - Tried to connect SSL
    - Attempts to brute force RPC data if RPC is found
* "--version-intensity [0-9]" : Sets the intensity level of a version scan to the specified value. O is only null port, 7 is default, 9 is all probe.

![6  nmap_versionScan](https://github.com/user-attachments/assets/fac7d350-18f3-40a9-a5bd-4ff4fbd85d11)
