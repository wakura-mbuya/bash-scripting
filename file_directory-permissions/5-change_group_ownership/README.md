# Changing Group Ownership
<ol>
	<li> Create a new group name **mygroup** using the command **groupadd** </li>
	<li> Create a new file named **group_file.txt** </li>
	<li> Check the current group ownersip of the file using **ls -l** </li>
	<li> Change the group ownership of **group_file.txt** to **mygroup** using the **chown** command </li>
	<li> Verify the new group ownership using **ls -l** </li>
	<li> Create a new user and add them to **mygroup** using the **useradd** and **usermod** commands </li>
	<li> Test accessing **group_file.txt with the newly added user to see if the group ownership change is applied correctly </li>
</ol>
