
<h1>Managing File Permissions Using Linux Commands</h1>


<h2>Description</h2>
In this lab I examined existing permissions on the file system. I determine if the permissions match the authorization that should be given. If they do not match, I modified the permissions to authorize the appropriate users and removed any unauthorized access.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux Commands</b>
- <b>Document displaying the file structure of directories and permissions of its files and subdirectories.</b> 

<h2>Environments Used </h2>

- <b>Linux</b>

<h2>Program walk-through:</h2>

<p align="left">
I Checked the  file and directory details. I used the {ls} command with the
-{la} option to display a detailed listing of the file contents that also returned hidden files. The
output of my command indicates that there is one directory named {drafts}, one hidden file
named {.project_x.txt}, and five other project files. The 10-character string in the first
column represents the permissions set on each file or directory: <br/>
<img src="https://imgur.com/SCQVVBt.png" height="80%" width="80%" alt="File Permissions Step"/>
<br />
<br />

I determine whether any files have incorrect permissions and changed the permissions as needed using the {chmod} command. This action removed unauthorized access and strengthened security on the system: <br/>

I Check whether any files in the projects directory have write permissions for the owner type of other.{
project_k.txt}

<img src="https://imgur.com/Nvrazrt.png" height="80%" width="80%" alt="File Permissions Steps"/>
<br />
<br />

I Changed the permissions of the file identified in the previous step so that the owner type of 'other' doesn’t have write permissions.{project_k.txt}

<img src="https://imgur.com/JXKYqCf.png" height="80%" width="80%" alt="File Permissions Steps"/>
<br />
<br />
The file "project_m.txt" is a restricted file and should not be readable or writable by the 'group' or 'other'; only the user should have these permissions on this file Therfore, Listed the contents and permissions of the current directory and checked if the 'group' had read or write permissions.

<img src="https://imgur.com/eerwyPO.png" height="80%" width="80%" alt="File Permissions Steps"/>
<br />
<br />
I Used the {chmod} command to change permissions of the project_m.txt file so that the group doesn’t have read or write permissions. I then used {ls -la} to review the updates I made.
<img src="https://imgur.com/tY1a2mG.png" height="80%" width="80%" alt="File Permissions Steps"/>
<br />
<br />











</p>
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

