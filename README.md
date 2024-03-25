<h1>Auditing and editing file permissions for users (employees) in Linux Command Line</h1>


<h2>Description</h2>
I am a security professional at a large corporation working as part of the research team. Part of my job is ensuring that all users on the team are authorized with the correct and appropriate permissions set out by the organization. This helps keep the system secure. I will be examining existing permissions on the file system. I will be ensuring that the permissions given match the permissions authorized by the organization. If they do not match, using Linux commands, I will be modifying the permissions and removing unauthorized access.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux Command Line</b> 


<h2>Program walk-through:</h2>



<h1 align="center">Check file and directory details: </h1>
  
The /home/researcher2/projects directory must be checked to examine the permissions authorized for the directory and files it contains. 

<img src="https://i.imgur.com/orUzIQ5.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>

After navigating to the projects directory using the command cd projects, the permissions for the directory and the files within the directory can be viewed by executing the ls -la command. The -la command will also show hidden files and directories. Whereas -l will only show files and directories which are not hidden.

<img src="https://i.imgur.com/otB9u62.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>


<h1 align="center">Describe the permissions string:  <h1/>


<img src="https://i.imgur.com/SEdB1he.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>

The above screenshots shows the permissions for the file .project_x.txt. The permissions string -rw—w---- can be broken down into 10 separate strings or characters. The - at the beginning of the permissions string indicates these are permissions for a file and not a directory. A directory permissions string would begin with the letter d. Following this are the permissions for the three user types. The first 3 strings grouped together rw- show the permissions for the user. r referring to read, w referring to write and x finally referring to the ability to execute executable files. The - means the permission is missing for the file or directory. The second group of 3 strings show the permissions for the group. In this screenshot -w- shows that the group only has write permissions for this file. Finally, the last 3 strings — demonstrate that the other users have neither read, write or executable permissions.

<br />
Change file permissions: <br/>
<img src="" height="80%" width="80%" alt="Editing Linux Permissions steps"/>
<br />
<br />
Change file permissions on a hidden file:  <br/>
<img src="" height="80%" width="80%" alt="Editing Linux Permissions steps"/>
<br />
<br />Change directory permissions:  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>
<br />
<br />
Summary:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Editing Linux Permissions steps"/>
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
