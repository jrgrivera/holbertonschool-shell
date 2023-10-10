su - Switches the current user to the user "betty"
whoami - Prints the effective username of the current user
groups - Prints all the groups current users us part of
chown - To change the user of the file 'name' to the user 'name' 
touch - Create an empty file
chmod 744 - To execute permission to the owner of the file
chmod - u+x (execute permission to the owner), g+x (the group of the owner), o+r (read permission to other users for the file)
chmod ugo+x (execution permission to the owner, the group owner, and other user for the file)
chmod 007 (set the permissions owner: no permission at all, Group: no permission at all, Other users: all the permissions)
chmod 733 (set the mode of the 'file' 
chmod --reference=olleh hello - Set the mode of the 'hello' file the same as the 'olleh' file
find . -type d -exec chmod ugo+x {} +  -  To add execute permission to all subdirectories of the current directory for the owner, the group owner, and all other users while leaving regular files unchanged
mkdir -m 751 my_dir   -  Create the directory "my_dir" with permissions 751 in working directory
sudo chown :school hello   -  Change the group owner of the file "hello" to "school" in the working directory
sudo chown -R vincent:staff  -  Change the owner to "vincent" and the group owner to "staff" for all files and directories in the working directory
sudo chown vincent:staff _hello   -  Change the owner and group owner of the symbolic link "_hello" to "vincent" and "staff", respectively
