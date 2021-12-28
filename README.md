##### nmap
Default NMAP behaviour depends on **privileges** :
- Privileged (root/Administrator*)
  - TCP SYN scan
- Unprivileged
  - TCP connect scan  

masscan огенемёт
nmap скалпель

``` python tnmap.py 122.64.0.0/11 | xargs -I CMD nmap -sT -sV -sC -n -vvv -Pn -min-rate=1000 --min-hostgroup=256 -oX - CMD ```
