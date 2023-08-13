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



    
  id: The id command displays the real and effective user and group IDs associated with the current user. It provides information about your identity and group memberships.

   whoami: The whoami command simply displays the username of the current user. It's a quick way to confirm your identity.

  hostname: The hostname command shows the system's host name. You can use it to identify the name of the machine you're on.
    
  uname: The uname command provides system information like the kernel version, machine hardware, and operating system. Common options include:
        -a: Displays all available information.
        -r: Shows the kernel release.
        -s: Prints the kernel name.

   ps -ef: The ps command with the -ef flags displays a snapshot of the current processes running on the system. This can help you identify running services and processes.

  echo $PATH: This command prints the value of the PATH environment variable, which specifies the directories where executable files are located. It's essential for understanding where your shell looks for commands.

   ifconfig: The ifconfig command is used to configure network interfaces and display network-related information such as IP addresses, subnet masks, and more. Note that on modern systems, the ip command has largely replaced ifconfig.

 cat /etc/passwd: This command displays the contents of the /etc/passwd file, which contains information about user accounts on the system, such as usernames, user IDs (UIDs), and home directories.

   sudo -l: The sudo -l command lists the commands that a user can execute with sudo privileges. It's useful for identifying potential paths to privilege escalation.

  find / -type f -a −perm−u+s−o−perm−g+s−perm−u+s−o−perm−g+s -exec ls -l {} ; 2> /dev/null: This command searches the entire file system for files that have the setuid (suid) or setgid (sgid) permissions set. Files with these permissions can potentially lead to privilege escalation. The ls -l command is used to display detailed information about each file found.
