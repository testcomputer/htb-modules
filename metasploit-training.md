msfconsole: The main command-line interface.
Modules: supporting modules such as exploits, scanners, payloads, etc.
Tools: Stand-alone tools that will help vulnerability research, vulnerability assessment, or penetration testing. 
Some of these tools are msfvenom, pattern_create and pattern_offset. We will cover msfvenom within this module, 
but pattern_create and pattern_offset are tools useful in exploit development which is beyond the scope of this module. 


![image](https://github.com/testcomputer/HackTheBox-Modules/assets/104815254/4672edd1-f286-4a04-848b-6b24c6cf5b12)

practice this format when searching msf6

      search type:exploit platform:windows cve:2021 rank:excellent microsoft

we could specify the year (cve:<year>), the platform Windows (platform:<os>), the type of module we want to find (type:<auxiliary/exploit/post>), the reliability rank (rank:<rank>), and the search name (<pattern>). This would reduce our results to only those that match all of the above.
