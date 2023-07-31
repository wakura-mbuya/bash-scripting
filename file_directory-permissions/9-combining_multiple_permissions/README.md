
# Combining Multiple Permissions
<ol>
	<li> Create a new directory name **shared_dir** </li>
	<li> Set the permissions of **shared_dir** to give read, write, and execute permissions to the owner and the group, and only read and execute permissions to others using octal notation </li>
	<li> Verify the permissions using **ls -ld** </li>
	<li> Create a new file inside **shared_dir** and set its permissions to give read and write permissions to the owner, read-only permissions to the group, and no permissions to others using octal notation </li>
	<li> Verify the permissions using **li -l** </li>
	<li> Test accessing and modifying the file using different user accounts to ensure the combination of permissions works as expected </li>
