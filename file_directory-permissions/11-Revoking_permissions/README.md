# Revoking Permissions
<ol>
	<li> Create a new file name **revoke_file.txt** </li>
	<li> Set the permissions of **revoke_file.txt** to give read and write permissions to the owner, read and write permissions to the group, and read-only permissions to others using octal notation. </li>
	<li> Verify the permissions using 'ls -l' </li>
	<li> Use symbolic notation to revoke the write permissions for the owner and the group, but keep the read permissions intact. </li>
	<li> Verify the new permissions using 'ls -l' </li>
	<li> Test accessing and modifying **revoke_file.txt** using different user accounts to ensure the permissions are revoked accordingly </li>
