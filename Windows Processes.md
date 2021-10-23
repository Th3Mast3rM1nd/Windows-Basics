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

<img width="650" alt="Screen Shot 2021-10-23 at 20 02 50" src="https://user-images.githubusercontent.com/92652606/138567287-a360776c-0995-4b75-a2e9-e521203c527e.png">

``` tasklist /FI "pid eq number" ``` : search for a processe using Pid number 

<img width="668" alt="Screen Shot 2021-10-23 at 20 04 53" src="https://user-images.githubusercontent.com/92652606/138567290-30aa9a63-d37e-4047-aa78-ee67f09830b1.png">


```/FI ```: Using filter
:
1. USERNAME 
2. PID
3. IMAGENAME 
4. STATUS ( RUNNING | SUSPENDED | UNKNOWN | NOT RESPONDING )

<img width="706" alt="Screen Shot 2021-10-23 at 20 10 01" src="https://user-images.githubusercontent.com/92652606/138567296-7ff3f95a-2965-42f0-8f8c-1f96e8b77d29.png">

Valid Operators 
:
1. eq ( equal) ne ( not equal) gt ( greater than ) lt ( lessthan )

<img width="1368" alt="Screen Shot 2021-10-23 at 20 11 35" src="https://user-images.githubusercontent.com/92652606/138567308-184496ea-62a8-4583-84be-c1c4c213b199.png">

```/V``` : Verbose mode 

We can use as well ```tasklist``` and ```find```to find a name of a Processess 

<img width="627" alt="Screen Shot 2021-10-23 at 20 13 19" src="https://user-images.githubusercontent.com/92652606/138567324-b0dd7237-c8a8-460e-98f6-14ce616a9afc.png">


```taskkill```: to kill a Proccess 

 <img width="737" alt="Screen Shot 2021-10-23 at 20 15 28" src="https://user-images.githubusercontent.com/92652606/138567311-4a899b2d-9e8b-46ed-af9b-47ea927fee3b.png">




