# Port Scan

By default nmap check is the top 1000 ports used on the internet. 

| Options | Description |
|---------| -------------|
| -- top-ports [#] | Specify the # of the ports to scan |
| -p 21,22,25 | multipul ports at the same time |
| -p 1-32,80,50-55,443 | range of ports |
| -p 0-65535 | All ports in the entire networks |

*Note: "-r" to scan them in order, default is randomized*

### Example:

![4  nmap_portscanning](https://github.com/user-attachments/assets/fe76c1dd-b327-4881-b1a4-4ed4b79dacfa)

