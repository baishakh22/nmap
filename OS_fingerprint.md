# OS Fingerprint

Nmap offers active OS fingerprinting

* Sends specially crafted packets to target to measure response.
* Performs many tests.
* Details: https://nmap.org/book/osdetect-methods.html#osdetect-response-tests


| Options | Description |
| --------| ------------| 
| -O | enables OS Fingerprinting |
| --osscan-limit | Limits OS fingerprinting to promising targets |
| --osscan-guess | Aggressively guesees the OS, even if low-confidence |


## Example:

```
sudo nmap -Pn -sS -O 10.10.0.5 -p 21,22,25
```

![5  nmap_OSfingerprint](https://github.com/user-attachments/assets/7cda218c-6445-42fa-90b3-5ffbf8e26989)

 
