# Local Accounts & Groups 
Local user accounts are stored locally on the server. These accounts can be assigned rights and permissions on a particular server, but on that server only. Local user accounts are security principals that are used to secure and manage access to the resources on a standalone or member server for services or users. The Three Imporatant local Accounts are : 

1. Administrator account : <p> Administrator is a user account designed for the system administrator to manage the machine. Its SID is always S-1-5-domain-500. The Administrator has full permissions on all files and directories on the machine. This makes it an especially desired target during penetration tests and security audits. It’s important to note that the Administrator account is disabled by default on Windows 10. During initial account creation, another user account will usually be assigned administrative permissions to act in its stead. Such permissions are provided by means of membership to the Local Administrators group.</p>
2. Guest account :<p>The Guest account lets non-users of the machine log on temporarily with restrictive permissions. It belongs to the Guests group, with SID S-1-5-32-546. By default, the Guest account is disabled, but when enabled it often has a blank password. It's important to note the implications of this from a security perspective, because if the guest account on a victim has been enabled, we can often log on to it.</p>

3. SYSTEM account : <p> The SYSTEM account is used by the OS to run services that need elevated permissions. By default, it has all the permissions of the Administrator, but it isn't supposed to be logged-in to by a human user. That being said, some exploits can allow us to execute code in the context of its owner. If a process running as SYSTEM gets exploited, we might be able to impersonate the SYSTEM user itself.</p>

```net```: used to create , add or delete user account and groups membership .

```net /user ```: to print all the users on the machine.
screen shot 

```net user /add ``` : to add a user to the machine.

screen shot 

```net user USERNAME``` : to display Information about a User.

screen shot 

```net localgroup ``` : to print the local groups on the machine 

screen shot 

```net localgroup /add Groupname  ``` : to add new Group 

screen shot 

```net localgroup GroupName Username /add ``` : to add a User to a localgroup 

sceen shot 

```net localgroup /del Groupname ``` : Delete The Group 

screen shot 

```net user /del Username ```: to delete a user from the System 

scren shot 

```net accounts ``` to see or  user account Policies .



   
