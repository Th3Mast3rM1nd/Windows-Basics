# Dynamic Link Libraries ( DLL )
Libraries are repositories of functions that can easily be imported into other programs. Windows uses Dynamic-Link Libraries (DLLs),1 which are themselves actually written in the same format as .exe files. This helps eliminate reprogramming the wheel, so to speak, and also creates a bedrock of community and interdisciplinary collaboration. In this section, we'll cover some of DLLs that are commonly invoked by various processes.

Windows makes use of a significant number of shared libraries, which are called DLLS. DLLs contain code and data that can be called upon at the same time by more than one program. DLLs essentially allow a program to call upon already-written functionality instead of needing to perform those functions itself.

On 64-bit versions of Windows, DLLs and system executables are stored in System32 and SysWOW64. As we touched on in a previous section, System32 contains 64-bit libraries and SysWOW64 contains 32-bit libraries. On 32-bit version of Windows, all system-wide libraries are located in System32.

Let's go over a short list of common Windows DLLs and their basic functionality:

***HAL.DLL***: The Hardware Abstraction Layer is a Kernel mode library file and it cannot be used by any User mode programs. It performs multiple functions related to the system's underlying hardware.

***NTDLL.DLL***: The New-Technology DLL allows User mode programs to call upon the Windows Native API.2 The Native API is used when other more robust APIs are unavailable, such as during system startup. For example, the aformentioned csrss.exe calls upon NTDLL.DLL functionality.

***KERNEL32.DLL***: This DLL allows applications to call upon most of the Win32 base APIs involving things like memory management, input and output operations, and more. As an example of how DLLs can be used by other code, KERNEL32.DLL itself implements much of its functionality by calling upon NTDLL.DLL code.

***USER32.DLL***: Allows applications to call upon objects making up the user interface, like the desktop, taskbar, and Start menu.

***ADVAPI32.DLL***: Allows applications to call upon security features as well as functions that manipulate the Registry. 

There are many more DLLs that Windows runs on.

Find Dlls Files using command line : 

<img width="544" alt="Screen Shot 2021-10-24 at 13 27 56" src="https://user-images.githubusercontent.com/92652606/138592158-e504480b-2f1d-46ef-a096-28e690e38086.png">
