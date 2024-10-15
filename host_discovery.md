## Nmap Host Discovery

![Screenshot 2024-10-12 at 2 24 31 PM](https://github.com/user-attachments/assets/6c37ea80-d705-42c4-80a0-538f8759b6a5)

```
-sn: Ping Scan. It will disable the port scan. So no port scan. 
-Pn: Treat all hosts as online. This will skip the host discovery. 
```

Example:

```
nmap -sn 10.10.0.5
nmap -Pn 10.10.0.5
```
![2  nmap_hostdiscovery](https://github.com/user-attachments/assets/5369c6f0-7926-4ba0-a639-734b6c3ec096)

