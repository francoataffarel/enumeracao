Enumeração

Enumeração de portas

nmap -p- -Pn -n <ip>

rustscan <ip> --no-nmap

Enumeração de total:

nmap -A -p 21,22,80,445,8080 -Pn -n <ip>

nmap -A --top-ports 1500 -Pn -n <ip>

rustacan <ip> -- -A -sC -ulimit 5000

Caso esteja executando ssh -D:

proxychains nmap --unprivileged comandos


Enumeração da porta 445:

Listas as pastas shareds: smbclient -N ////<ip>//

Lista a pasta selecionada: smbclient -N ////<ip>//<pasta shared>

Lista a pasta selecionada(smbmap):  smbmap - H <ip> -U anonymous -s <pasta shared>

dirb <ip>

nikto -h  <ip>

wfuzz >> preencher




