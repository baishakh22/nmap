## SCAN TECHNIQUES

Some scan need a root level access for packet crafting and sniffing

### TCP scan

| Option | Types | Description |
|-------| -------| ------------|
| -sS | SYN | Default UID0: Stealthy half-open, doesn't complete 3-way handshake |
| -sT | Connect | Default non-privileged: 3-way handshake, slow, likely to be logged by HOST |
| -sA | ACK | Unreliable scan, helps to get around firewalls blocking incoming SYN |
| -sF | FIN | FIN set |
| -sN | Null | No control bits |
| -sX | XMAS | FIN, PSH, URG |
| -sW | Windows | Windows operating system |
| -sM | FIN ACK | Maimon, some BSD, systems respond with an RST if closed |
| --scanflags  <flags>: | [URG/ACK/PSH/RST/SYN/FIN/ECE/CWR/ALL/NONE] | Customize TCP scan flags | 


![3  nmap_scanTechniqueTCP](https://github.com/user-attachments/assets/c26b4366-b558-4ef7-8867-844a6d675dda)


### UDP Scan
Less options since UDP does not have control bits
Sends port-specific payloads or no payload, as applicable


| Option | Types | Description |
|-------| -------| ------------|
| -sU | UDP | UDP Scan |


Common Ports get a payload to help facilitate a response

| 7 | echo |
|----| ----|
| 53 | DNS |
| 123 | NTP |
| 137 | netbios |
| 161 | snmp |



![3  nmap_scanTechniqueUDP](https://github.com/user-attachments/assets/d367b3c4-03ac-4d1d-aef6-ab9ebb2ddeeb)


### *Note:*
* <code style="color : red">nmap is dynamic and will automatically slow down.</code> ⬆️ 
* Scan status requested one per second.
* Linux only sends one ICMP Unreachable per second.
* In the screenshot, I specify the top 100 ports, otherwise it will get forever. 
