# Sticky Bit for Shared Directories
<ol>
	<li> Create a new directory name **sticky_dir** </li>
	<li> Set the permissions of **sticky_dir** to give read, write, and execute permissions to the owner, the group, and others using octal notation </li>
	<li> Vevify the permissions using 'ls -ld' </li>
	<li> Enable the sticky bit on **sticky_dir** to prevent users from deleting files that do not belong to them using octal notation </li>
	<li> Verify the new permission using 'ls -ld' </li>
	<li> Create a new file inside **sticky_dir** and set its permissions to allow read and write for all users </li>
	<li> Test deleting the files using a different user account to see if the sticky bit restricts deletion </li>
