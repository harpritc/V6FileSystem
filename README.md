# UNIX V6FileSystem

Objective 
To design and develop a program called fsaccess which will allow a Unix user access to the file system of a foreign operating system, the modified Unix Version 6 or mV6.

This modified file system will support the following commands 

Initfs - For initializing the file system. 
cpin - Creating a file using modified v6 file system. 
cpout - For copying the contents of a file in the file system to an external file 
mkdir - Creating directory using this file system. 
q - Save and quit the file system. 
Format of Commands and their functionalities 

initfs /path/in/disk n1 n2. 
n1 - represents the total number of blocks in the disk. 
n2 - represents the total number of i-nodes in the disk.

cpin externalfile mv6-file 
This command should create a new file called v6-file in the current directory of the v6 file system and fill the contents of the newly created file with the contents of the external file. 

cpout mv6-file externalfile 
If v6-file exists, the command will create external file and copies the contents from v6-file to the external file. If v6-file is not present in the file system it will display an error message in the console. 

mkdir mv6-dir 
If v6-dir is not already present in the v6 file system, a new directory is created. If the directory is already present in the file system, an error message will be displayed in the console. 

q
Save all changes and quit.
