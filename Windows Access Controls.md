# User Account Control (UAC)

User Account Control (UAC) helps prevent malware from damaging a PC and helps organizations deploy a better-managed desktop. With UAC, apps and tasks always run in the security context of a non-administrator account, unless an administrator specifically authorizes administrator-level access to the system. UAC can block the automatic installation of unauthorized apps and prevent inadvertent changes to system settings.

[ How User Account Control Works ](https://docs.microsoft.com/en-us/windows/security/identity-protection/user-account-control/how-user-account-control-works)

picture 

# Security Identifier (SID)

SIDs are alpha-numeric codes that uniquely identify principals on a Windows machine. Some SIDs are considered well-known, and they identify the same principal on every Windows OS. An example of a well-known SID is S-1-1-0, which belongs to the Everyone group. This SID includes all users on the machine.

```whoami /user ``` : to see the SID of the logged User 

screen shot 

| Number | Meaning | Description 
|--------|---------|--------------
| s | SID | Indicates that the string is a SID
| 1 | R | Indicates the revision level
|5 | X | Indicates the identifier authority value 
| 21 | Y | Represents a series of subauthority values, where n is the number of values


