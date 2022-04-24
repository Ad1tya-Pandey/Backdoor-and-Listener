# Backdoor-and-Listener
*This repository consists of a Backdoor program and a listener which would help a host execute commands remotely* 
on the victim System 
This project consists of two components 1)backdoor 2) Listener.
both the mentioned programs are built in python and work together in acheiving
the task of remote execution of commands on a victim system  in LAN (Local area Network).

->Backdoor -A backdoor is a malware type. that negates normal authentication procedures to access a system.
As a result, remote access is granted to resources within an application, such as databases and file servers,
giving perpetrators the ability to remotely issue system commands and update malware.
 
->listener-listener  is a computer networking utility for reading from and writing to network connections 
using TCP which in this case would serve as a component which would
listen to the incoming connections from the backdoor and would channel the provided 
commands through the network stream and their respective output.
 
Here the backdoor connects back to the listener using a reverse TCP connection
from the mentioned port in the program . addtionally the python file is been converted into an executable (.exe)
file so that it could be attached  with any of the multimedia or
software resulting into obfuscated execution of the backdoor as the main program is 
executed.


what makes it different:
-This backdoor doesn't run in the foreground and hence isn't visible to the user making it  quite stealthy.
-It also is persistent after being executed for once on the victim machine hence gives ease of access even when the system reboots.
-It estabilishes  a reverse Tcp connection to the listener making it bypass the firewall with ease. 
-Has functionality of downloading and uploading files in addition to executing system commands on the victim machine.


### when combined with a crypter this backdoor would become fully undetectable , i'd be uploading a crypter program soon in future ###
**DISCLAIMER-This backdoor is made solely for educational ,ethical and awareness purposes . i don not take responsibility for it being used / modified maliciously for execution without the permission of respective system owner .**
