# Local Accounts & Groups 
Local user accounts are stored locally on the server. These accounts can be assigned rights and permissions on a particular server, but on that server only. Local user accounts are security principals that are used to secure and manage access to the resources on a standalone or member server for services or users. The Three Imporatant local Accounts are : 

1. Administrator account : <p> Administrator is a user account designed for the system administrator to manage the machine. Its SID is always S-1-5-domain-500. The Administrator has full permissions on all files and directories on the machine. This makes it an especially desired target during penetration tests and security audits. It’s important to note that the Administrator account is disabled by default on Windows 10. During initial account creation, another user account will usually be assigned administrative permissions to act in its stead. Such permissions are provided by means of membership to the Local Administrators group.</p>
2. Guest account :<p>The Guest account lets non-users of the machine log on temporarily with restrictive permissions. It belongs to the Guests group, with SID S-1-5-32-546. By default, the Guest account is disabled, but when enabled it often has a blank password. It's important to note the implications of this from a security perspective, because if the guest account on a victim has been enabled, we can often log on to it.</p>

3. SYSTEM account : <p> The SYSTEM account is used by the OS to run services that need elevated permissions. By default, it has all the permissions of the Administrator, but it isn't supposed to be logged-in to by a human user. That being said, some exploits can allow us to execute code in the context of its owner. If a process running as SYSTEM gets exploited, we might be able to impersonate the SYSTEM user itself.</p>

```net```: used to create , add or delete user account and groups membership .

```net /user ```: to print all the users on the machine.

<img width="638" alt="Screen Shot 2021-10-23 at 16 13 15" src="https://user-images.githubusercontent.com/92652606/138560664-df6bd3f2-31a7-45bf-8714-05bcba89524d.png">

```net user /add USERNAME PASSWORD ``` : to add a user to the machine.

<img width="703" alt="Screen Shot 2021-10-23 at 16 16 10" src="https://user-images.githubusercontent.com/92652606/138560672-1b86ecce-6be5-41ae-86b6-653e857c85a9.png">

```net user USERNAME``` : to display Information about a User.

<img width="522" alt="Screen Shot 2021-10-23 at 16 17 41" src="https://user-images.githubusercontent.com/92652606/138560685-82fd605a-770b-4e6c-a603-f71a57530311.png">

```net localgroup ``` : to print the local groups on the machine 

<img width="463" alt="Screen Shot 2021-10-23 at 16 18 55" src="https://user-images.githubusercontent.com/92652606/138560690-4c759eb9-13a0-4168-8f67-124353428aa1.png">

```net localgroup /add Groupname  ``` : to add new Group 

<img width="521" alt="Screen Shot 2021-10-23 at 16 21 23" src="https://user-images.githubusercontent.com/92652606/138560695-84837210-206b-4b2c-9bf2-ab61da477612.png">

```net localgroup GroupName Username /add ``` : to add a User to a localgroup 

<img width="652" alt="Screen Shot 2021-10-23 at 16 22 51" src="https://user-images.githubusercontent.com/92652606/138560706-ad5d27c1-20b1-437f-bf68-e13935f1cbe1.png">

```net localgroup /del Groupname ``` : Delete The Group 

<img width="530" alt="Screen Shot 2021-10-23 at 16 25 17" src="https://user-images.githubusercontent.com/92652606/138560728-8743c0de-72f6-442b-8e51-b3e8213d6152.png">


```net user /del Username ```: to delete a user from the System 

<img width="554" alt="Screen Shot 2021-10-23 at 16 25 47" src="https://user-images.githubusercontent.com/92652606/138560745-d6cd28fd-6d84-48f9-ac52-88c2a63dede2.png">

```net accounts ``` to see or  set a user account Policies .

<img width="570" alt="Screen Shot 2021-10-23 at 16 27 34" src="https://user-images.githubusercontent.com/92652606/138560748-9bd823c3-222d-4b8f-867c-6d1a2d5be62a.png">

```runas ```: is a command used to run a command as another User but works just if you have GUI access to the target machine like using rdp 

<img width="569" alt="Screen Shot 2021-10-23 at 16 50 08" src="https://user-images.githubusercontent.com/92652606/138561254-a613ccae-6ecf-4225-bb89-22fe3aed9e72.png">



