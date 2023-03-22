Target Machine (Objective's IP Address) = 10.129.66.65

Enumeration
Just as usual, we start off with the Nmap scan:

    nmap -sC -sV 10.129.66.65
    
Starting Nmap 7.93 ( https://nmap.org ) at 2023-03-21 21:05 MDT
Nmap scan report for 10.129.66.65

![image](https://user-images.githubusercontent.com/104815254/226791929-fcca7e65-5538-4fc3-829d-6cf78626f7f0.png)



Scanning their network we are able to see open ports.
Port 21(TCP) FTP
Port 22(TCP) SSH
Port 80(TCP) HTTP



![image](https://user-images.githubusercontent.com/104815254/226792261-0afd6899-daf6-4570-a25b-c773dc17504f.png)
