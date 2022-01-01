### nmap vs masscan
[hack5](https://www.youtube.com/watch?v=7XMIFTRiAGA&t=1654s)

masscan огенемёт nmap скалпель

[tasa](https://github.com/PaulMcMillan/tasa/blob/master/examples/tnmap.py)

``` python tnmap.py 122.64.0.0/11 | xargs -I CMD nmap -sT -sV -sC -n -vvv -Pn -min-rate=1000 --min-hostgroup=256 -oX - CMD ```

### Fingerprinting своим руками

### Fingerprinting своим руками

### basic
Default NMAP behaviour depends on **privileges** :
- Privileged (root/Administrator*)
  - TCP SYN scan
- Unprivileged
  - TCP connect scan  

masscan огенемёт
nmap скалпель

``` python tnmap.py 122.64.0.0/11 | xargs -I CMD nmap -sT -sV -sC -n -vvv -Pn -min-rate=1000 --min-hostgroup=256 -oX - CMD ```

- Script scan -sC
  - Equivalent to --script=default
 - --script accepts:
   - Filename
   - Directory
   - Category
   - Expressions
 
Script Categories:
- auth
- broadcast
- brute
- discovery
- dos
- exploit
- external
- fuzzer
- intrusive
- malware
- safe
- version
- vuln

Expressions are supported:
- --script="default or save"
- --script="(default and save) and not http-*"

### NSE scripting (Nmap Scripting Engine)
https://www.youtube.com/watch?v=M-Uq7YSfZ4I&t=19s
- Service
  - executed once per port
- Host
  - executed once per host
- Pre-rule
  - executed prior and scan
- Post-rule
   - executed after all scans
 
 
