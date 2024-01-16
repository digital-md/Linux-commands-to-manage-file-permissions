<h1>Linux Commands to Manage File Permissions</h1>

<h2>Description</h2>
At my organization, the research team needs to update the file permissions and directories in the system. I will go into the projects directory and make sure the users have the appropriate permissions and update those necessary to provide a more secure system. The permissions currently do not match the level of authorization provided. Making sure you check the system and update it will help keep it secure. To complete this, I will perform the following tasks. See below 
<br />

<b>Check file and directory details</b> 

The following codes demonstrate how Linux commands were used to update the permissions in the directories in the system files.

![image](https://github.com/digital-md/Linux-commands-to-manage-file-permissions/assets/156498985/5390cbae-7250-43eb-b7e0-46df02c6f537)

In the first line, it describes the command line I used; the remaining line is the output. This code lists all of the contents within the project's directory. I used the ls command combined with the -la option to display all contents including hidden files. The output of my command displays that there is a drafts directory, a hidden file .project_x.txt, and six (6) other files. The first 10 characters in the string represent the permissions the user, group, and others have on each file or directory. 

<b>Describe the permissions string</b>

The 10 characters at the beginning of the string can be constructed to determine who has access to that file and/or directory as well as who may have specific permissions. 
1st character- If the first character is a d it is a directory. If it is a – then it is a file. 
2nd through 4th characters- If the character is a r it means read, if it is a w it means write, and if it is an x that means execute these permissions for the user.  If there is a hyphen – that means that no permissions are granted to the user. 
5th through 7th characters- The character r means read, w means write, and x means execute permissions for the group. If there is a hyphen – no permissions are granted for the group. 
8th through 10th characters- If it is r means read, the w means write, and x means execute permissions for others. Additionally, if there is a hyphen – there is no permission granted to others. 
For example: For project_r.txt , the first 10 characters are -rw-rw-r—that means this is a file the user has reading and writing permissions, the group has reading and writing permissions and others have only reading permissions. 

<b>Change file permissions</b>

The organization had decided that in file project_k.txt the other should not have writing permissions. Therefore, you can see In the string how it was changed. I used the chmod command to change it, o for other, and – subtract w for writing permissions from project_k.txt file. Additionally, in the file project_m.txt the group was not to have reading permission. I used the chomd command once again and g for group hyphen – for subtracting the r for reading and the file name to change this. After I used ls -la to review the updates.  Here is the string with a list of Linux commands used to change file permissions. 

![Screenshot 2024-01-16 013534 chmod](https://github.com/digital-md/Linux-commands-to-manage-file-permissions/assets/156498985/31883a54-200d-416f-a383-b9a523ecddf7)

<b>Change file permissions on a hidden file</b>

Here we have a hidden file .project_x.txt, with the current permissions -rw—w---- the organization let the research team know that this hidden file should not have permissions to write at all. I was notified to make the file readable for the user and group only. We used the chmod command to change the permissions. Then u for user – hyphen to subtract, like so u-w to remove writing privileges for the user and g-w to remove writing permissions for the group. We next listed the hidden file.project_x.txt for the file path that needed to be modified.  After completing it I used the ls -la to review the update.  


- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
