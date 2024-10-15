# Nmap Scripting Engine (NSE)

* NSE allows developers to write and release free scripts to argument and improve Nmap's functionality.
* Write in Lua
    - Run scripts in parallel using nmap multithreaded architecture.
    - Support network discovery, improve version scanning and OS detection.
    - Interact with targets to get more information.
    - Perform vulnerability scanning.
    - Detect malicious behavior, malware, backdoors.
    - Exploitation of vulnerabilities.


### Use

```
-sC
--script=[all,category,script]
```

### NSE Categories

| Option | Description |
| -------| ------------| 
| auth | Looks for authentication issues |
| broadcast | Uses broadcast messages to discover hosts |
| brute | Try brute forcing authentication  |
| default | The default scripts with -sC |
| discovery | Get info about your targets |
| dos | Tests targets for DoS, exploits if possible | 
| exploit | Looks for vulns and exploits them |
| external | Uses external databases or resources to get more info |
| fuzzer | fuzzes, DNS, html form, and PHP |
| intrusive | Tried many brute force attacks and exploits |
| malware | Looks for signatures/signs of malware or if host is known malicious |
| safe | All the scripts that are non-intrusive, non-damanging |
| version | Perform version detection, uses outside queries |
| vuln | Looks for many more vuln, not all have exploits |

![7  nmap_NSE](https://github.com/user-attachments/assets/8fc6b01b-5d15-4586-a089-a69bcad02fbd)
![8  nmap_NSE](https://github.com/user-attachments/assets/e2be0b20-17ef-4c07-99b3-64dad14fdf0c)
![9  nmap_NSE](https://github.com/user-attachments/assets/7e2fdfc5-a1e8-4efe-a618-75400b5f8a2f)
