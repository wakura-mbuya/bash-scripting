# Linux Files and Directories Permissions
In Linux OS, files and directories have permissions and ownership. Files and directory permissions and ownership determine who can access, modify, or execute files and directories. Properly managing permissions and ownership is crucial for maintaining security and controlling access to sensitive data.

### File Permissions
File permissions are represented using a 3-digit octal notation such as <em>(644 or 755)</em>, or a symbolic notation <em>(such as -rw-r--r-- or drwxr-xr-x)</em>. Each permission is represented by a single digit:
<ul>
	<li> <b>r</b>(Read): Allows reading the contents of the file </li>
	<li> <b>w</b>(Write): Allows modifying the file's content or deleting the file </li>
	<li> <b>x</b>(Execute): Allows executing the file (for scripts or executables program). </li>
</ul>
The permissions are set for 3 entities:
<ul>
	<li> Owner - the user who owns the file </li>
	<li> Group - A group of users with common permissions </li>
	<li> Others -All other users who are neither the owner nor part of the group </li>
</ul>

You can change file permissions using the <strong>chmod</strong> command. For example, to grant read and write permissions to the owner of the file:

'''
	chmod 600 file.txt
'''

### Directory Permissions
Directory permissions work similar to file permissions, the only key difference is <b>x</b> permission on a directory allows users to enter (cd) into the directory and access its contents. Without execute permission, users cannot access the directory's contents even if they have read permissions on the files inside.

### Ownership
Every file and directory in Linux is associated with an owner and a group. The  owner is the user who created the file, and the group is a collection of users with common permissions. The <b>chown</b> command is used to change ownership of the files and directories, while the 'chgrp' command is used to change the group ownership. for example, to change the owner of a file to user <em>john</em>:

'''
	chown john file.txt
'''

To change the group ownership of a file to the group <em>developers</em>:

'''
	chgrp developers file.txt
'''

### Special Permissions:
Linux also support special permissions such as <em>setuid, setguid</em> and <em>sticky bit</em>. The setuid and setgid permissions allow theuser executing the file to temporarily have the rights of the file owner or group, respectively. The sticky bit is often used on directories to restrict users from deleting files they do not own.

<ul>
	<li>
	<b>Setuid (SUID):</b> When the setuid permission is set on an executable file, the file is executed with the priviledges of the file's owner, not the user who executed it. This is often used for executable programs that need elevated permissions to perform specific tasks. For example:

'''
	chmod u+s executable_file
'''

	</li>
	<li>
	<b>Setgid(SGID):</b> When the setgid permission is set on an executable file or directory, the process or new files created within the directory inherit the group ownership of the parent directory rather thant the group of the user who created them. This is commonly used for shared directories where multiple users need group access. For example:

'''
	chmod g+s directory
'''

	</li>
	<li>
	<b>Sticky Bit: </b> The sticky bit is primarily used on directories to ensure that only the owner of a file can delete or rename it, even if other users have write permissions on the directory. This prevents users from tampering with each other's files in shared directories like <em> /tmp </em>. for example:

'''
	chmod +t directory
'''

	</li>

### Symbolic Notation for Permissions
Instead of using octal notation, you can set permissions using a symbolic notation using letters:
<ul>
	<li>**u**: Owner</li>
	<li>**g**: Group</li>
	<li>**o**: Others<li>
	<li>**a**: All (equivalent to **ogo**)</li>
</ul>
For example, to grant read and execute permissions to the owner and group of a file:

'''
	chmod u+rx, g+rx file.txt
'''

### Recursive Permission Changes
You can apply permission changes recursively to directories and their contents using the **-R** option with **chmod**. For example:

'''
	chmod -R u+r directory
'''

### Practical Exercises
This folder and its subdirectories contains practical exercises on Linux file Permissions. The tasks included are:
<ol>
	<li> Changing File Permissions </li>
	<li> Changing Directory Permissions </li>
	<li> Recursive Permissions </li>
	<li> Special Permissions </li>
	<li> Changing Group Ownership </li>
	<li> Symbolic notation for permission </li>
	<li> Restrictive Permissions </li>
	<li> Creating Secure Files and Directories </li>
	<li> Combining Multiple Permissions </li>
	<li> Setting Default Permissions with ACLs </li>
	<li> Revoking Permissions </li>
	<li> Sticky Bit for Shared Directories </li>
	<li> Managing Default Permissions with umask </li>
	<li> Understanding Special Permissions with Setuid and Setgid </li>
	<li> Securely Managing Sensitive Files </li>
</ol>

Each task is solved in a subfolder using bash scripts.
When running the bash scripts in the subfolders, be sure to run them in the correct order following the numbers in front of the script name
