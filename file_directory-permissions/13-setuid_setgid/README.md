# Understanding Special Permissions with Setuid and Setgid
<ol>
	<li> Create a simple shell script named **my_script.sh** with some commands (e.g. echo "Hello World") </li>
	<li> Check the permissions of the script using 'ls -l' </li>
	<li> Set the setuid bit on the script so that it runs with the owner's permissions using octal notation </li>
	<li> Verify the new permission using 'ls -l' </li>
	<li> Run the script with a different user and observe the output and behavior. </li>
	<li> Remove the setuid bit from the script </li>
	<li> Set the setgid bit on a directory of your choice and create new files inside it </li>
	<li> Verif the new permissions using 'ls -ld' and observe the group ownersip of the newly created files </li>
