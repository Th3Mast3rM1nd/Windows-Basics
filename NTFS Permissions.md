# NTFS Permissions 

New Technology File System (NTFS) the primary file system for recent versions of Windows and Windows Server—provides a full set of features including security descriptors, encryption, disk quotas, and rich metadata, and can be used with Cluster Shared Volumes (CSV) to provide continuously available volumes that can be accessed simultaneously from multiple nodes of a failover cluster.

[Check This Link for More Inforamtion about NTFS ](https://docs.microsoft.com/en-us/windows-server/storage/file-server/ntfs-overview)


1. NTFS allows faster access to external peripherals such as a USB drive.
2. NTFS supports larger files.
3. NTFS provides more security features.
4. NTFS allows faster formatting of drives.
5. NTFS is easier to configure.

``` NTFS Permissions : ```

Files 
:
| Permission | Description 
|------------| ------------
| read (R)   | Read the file and excute the file if its a script 
| Write (W)  | Write To the file but not delete the contents or the file 
| Read & Execute (RX) | read and excute file 
| Modify (M) | read and write and as well delete the file 
| Full Control (F) | read , write , change , delete the file 

Directories
:

| Permission | Description 
|------------| ------------
| read (R)   | list and view any file in the directory  
| Write (W)  | add files or subfolders to the directory 
| Read & Execute (RX) | allow to view and list files or subfolder in the directory and allwo excution of binaray files on the directory 
| Modify (M) | read and write and as well delete files and subfoders within the directory 
| Full Control (F) | read , write , change , delete 
| List Folder Contents | Users are permitted or denied permissions to view a listing of files and subfolders 
lay and change permissions on files and folders 

```icacls  Foldername or filename ``` to display permissions

<img width="503" alt="Screen Shot 2021-10-23 at 17 36 00" src="https://user-images.githubusercontent.com/92652606/138563093-259a21dd-fa31-425b-9ed4-78a88d3f4cd0.png">


``` icacls /T foldername /grant Username:(F)``` : to grant a user a permission on a folder or file 
```icacls /T ```: /T to set permission as well on the subfolders and files (recursively)

<img width="704" alt="Screen Shot 2021-10-23 at 17 40 13" src="https://user-images.githubusercontent.com/92652606/138563102-aea51909-5195-4c48-a072-716c7134af03.png">

```icacls filesnmae /deny Username:(F)``` : to delete a permission from a user.

 <img width="751" alt="Screen Shot 2021-10-23 at 17 45 01" src="https://user-images.githubusercontent.com/92652606/138563107-a3376001-348c-4b97-9a8b-05e0bd3da6fb.png">


