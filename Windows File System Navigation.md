# File System Navigation 

in Windows OS The root Directory is ```C:\ ```  and Other Drive are assigned Other Letter Like ```D:\ ``` , ```E:\``` ....
The C:\ Directory We can Call as well the boot Directory becuase From the OS start the booting . The Directory Structer Of The ```C:\```:
| Directory | Description 
|---------------|----------------|
|/Perflogs : |  Holds Preformance Logs but usely empty 
|/Program files : | On 32-bit systems, all 16-bit and 32-bit programs are installed here. On 64-bit systems, only 64-bit programs are installed here.
|/Program files (X86) : | 32-bit and 16-bit programs are installed here on 64-bit editions of Windows.
|/Program Data : | This is a Hidden Folder That Contains Program Data . The Data is accessed by the program no matter which users is logged in .
|/Users : | This Directroy Contains Users Profile 
|/Users/Default : | This is the default user profile template for all created users. Whenever a new user is added to the system, their profile is based on the Default profile.
|/Users/Public : | This Folder is accessible to all Users on the system . and as well shared Over the Network .
|/Users/Username/AppData :| This is a hidden subdirectory of \Users. It stores application data and settings for every user. \AppData contains three additional subfolders, namely \Roaming, \Local, and LocalLow. \Roaming is used for network-based logins for roaming profiles and synchronizes the user's data when they log in to the computer. The Windows per-user temporary directory,3 \Temp, can be found here under \Local.
|/Windows : | The most of the files required for the Windows operating system are in this Directory .
|System, System32, SysWOW64 : | This Folders Contains ( DLL) files and each time a program ask to load a dll windows looks in this Folders .
---------------------------------------------------------

### Lets Use The Command Line to navigate this Directories :
```Help``` : For more information on a specific command, type HELP command-name , when using Help without argument you will get all the command aviable .
Screen shot here 

Cd : Change Directories 
```mast3@DESKTOP-CN9CEF8 C:\Users\mast3>cd Desktop```

## cd\ : to back to the root Directory ```C:\``` 
```mast3@DESKTOP-CN9CEF8 C:\Users\mast3>cd\```
```mast3@DESKTOP-CN9CEF8 C:\>```

Dir : used to lo list the contents of the Current Directory 
Screenshot
Dir /A : List Hidden Folders or Files 
Sceen shot
Type : to read the content of a files
screen shot 

## to display How to use each of the command above you can use /?  or Help ```command```





