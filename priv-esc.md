Enumeration Commands 	Description
id 	print real and effective user and group IDs
whoami 	current user
hostname 	show or set the system's host name
uname 	print system information
ps -ef 	report a snapshot of the current processes
echo $PATH 	print environment PATH variable
ifconfig 	configure a network interface
cat /etc/passwd 	show passwd file contents
sudo -l 	list commands allowed using sudo
find / -type f -a \( -perm -u+s -o -perm -g+s \) -exec ls -l {} \; 2> /dev/null 	Find all files suid and sgid files
