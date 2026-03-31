# First Nmap Scan - Metasploitable 2

## Command Used
```bash
nmap -sV 192.168.56.101
```

## Raw Output
```text
PORT     STATE SERVICE VERSION
21/tcp   open  ftp       vsftpd 2.3.4
22/tcp   open  ssh       OpenSSH 4.7p1
23/tcp   open  telnet    Linux telnetd
80/tcp   open  http      Apache httpd 2.2.8
139/tcp  open  netbios-ssn Samba smbd
445/tcp  open  netbios-ssn Samba smbd
3306/tcp open  mysql     MySQL 5.0.51a
5432/tcp open  postgresql PostgreSQL DB
5900/tcp open  vnc
6667/tcp open  irc       UnrealIRCd
8180/tcp open  http      Apache Tomcat
```

## Security Findings
- Multiple legacy and vulnerable services exposed
- Cleartext services like Telnet detected
- Database services publicly reachable
- Legacy Samba services available
- Potential remote exploitation paths identified

## Risk Level
**Critical**
6000/tcp open  X11         (access denied)
6667/tcp open  irc         UnrealIRCd
8009/tcp open  ajp13       Apache Jserv (Protocol v1.3)
8180/tcp open  http        Apache Tomcat/Coyote JSP engine 1.1

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 12.01 seconds
