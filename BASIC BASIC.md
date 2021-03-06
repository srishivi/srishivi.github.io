# Basic Bash

> Bash scripts provide a way to interact with OS. 
> 
> Bash is default terminal for linux.

1. To connect to any server through terminal.
      `ssh root@ip`
     
   
2. useradd -m shivi

3. passwd shivi
   - provide `password`

4. To switch to the new user terminal
   su - username
   
5. Sample commands
   - date
   - cal
   - pwd
   - ls
   - To create a file : touch filename , vim filename
   - To read the contents of the file on the screen: cat filename.txt
6. To create and run a script
   - Create script.sh file
   - Run `bash scrip.sh`
7. `which` command is to know the location of the command.
    - For example `which ls`
8. echo$PATH : to know the path that is set in environment variables
9. `/` is the root directory for linux system.
10. home directory contains the user created for the system
    /home
11. to add in the path : $PATH=$PATH:~
12.  `ls -ltr` : To know the permissions on the files
    self group others
    - permission looks like -rw-rw-r-- 
13. chmod 666 scrpt.sh (#6 is binary for 110)
14. chmod +x scrript.sh : To give executable permission to all
15. #! /bin/bash 
    - This file is added at the top of a script to tell that this is a bash executable file.
    - file script.sh : command to check the type of the file

16. env command is to check all the environment variables.
17. ls -altr : all files are displayed
18. path=$PATH:/home/shivi can be set in .bashrc file for setting the env variable
19. `.` represent present working directory
20. `..` represent one directory back
21. above two folders are present in every directory as hidden directories.
22. 






   
     

 
   


   
