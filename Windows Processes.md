# Processes 
Here is some intersting processes
:
| Process | Descriptions 
|---------| -------------
|smss.exe | Session Manager SubSystem. Responsible for handling sessions on the system.
|winlogon.exe | loading the user Profile on logon . and authenticating users 
| csrss.exe | The Client Server Runtime Process is responsible for several background functions. It begins the shutdown sequence when terminated, and it is the parent of the process that eventually spawns cmd.exe.
| explorer.exe | Windows Explorer This is the process that gives the user access to their folders and files. It also provides functionality to other features such as the Start Menu, Taskbar
|wininit.exe | Windows Startup Starts the Wininit file .ini file that lists all of the changes to be made to Windows when the computer is restarted after installing a program.
| System | A background system process that runs the Windows kernel. 
|services.exe | loading services, interacting with services, starting/ending services 
| lsass.exe | Local Security Authority Subsystem Service responsible for enforcing the security policy on the system. It verifies users logging on to a Windows computer or server, handles password changes, and creates access tokens. It also writes to the Windows Security Log.
|svchost.exe  | Service Host is responsible for hosting and managing Windows services.


[ Check this PDF for more info about the Windows Processes  ](https://www.sans.org/posters/hunt-evil/)

``` tasklist ``` : list all processes on the machine

screen shot 

``` tasklist /FI "pid eq number" ``` : search for a processe using Pid number 
screen shot 

```/FI ```: Using filter
:
1. USERNAME 
2. PID
3. IMAGENAME 
4. STATUS ( RUNNING | SUSPENDED | UNKNOWN | NOT RESPONDING )

Valid Operators 
:
1. eq ( equal) ne ( not equal) gt ( greater than ) lt ( lessthan )

```/V``` : Verbose mode 


screnn shots 

We can use as well ```tasklist``` and ```find```to find a name of a Processess 

screen shot 

```taskkill```: to kill a Proccess 

scrren shot 



