# Setting Default Permissions with ACLs
<ol>
	<li> Create a new directory name **acl_dir** </li>
	<li> Set the permissions of **acl_dir** to give read, write, and execute permissions to the owner, read and execute to the group, and no permissions to others using octal notation </li>
	<li> Verify the permissions using **ls -ld** </li>
	<li> Enable Access Control Lists (ACLs) on **acl_dir** using the 'setfacl' command to allow specific additional users or groups to access the directory </li>
	<li> List the ACLs of **acl_dir** using 'getfacl' </li>
	<li> Test accessing and modifying **acl_dir** using both the owner and the added ACL users to see if the permissions are applied correctly </li>
