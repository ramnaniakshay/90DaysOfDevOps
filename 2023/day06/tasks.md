# Day 6 Task: File Permissions and Access Control Lists

### Today is more on Reading, Learning and Implementing File permissions

 The concept of Linux File permission and ownership is important in Linux. 
 Here, we will be working on Linux permissions and ownership and will do tasks on
 both of them. 
 Let us start with the Permissions.

1) Create a simple file and do `ls -ltr` to see the details of the files [refer to Notes](https://github.com/LondheShubham153/90DaysOfDevOps/tree/master/2023/day6/notes)

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/1e1fb311-43bd-46b6-9377-401448d716a5)


2) Each of the three permissions are assigned to three defined categories of users. The categories are:
-	   owner   —   The owner of the file or  application.
-	"chown" is used to change the ownership permission of a file or directory.
-	   group   —   The group that owns the file or application.
-	"chgrp" is used to change the group permission of a file or directory.
-	   others  —   All users with access to the system. (outised the users are in a group)
-	"chmod" is used to change the other users permissions of a file or directory.

    As a task, change the user permissions of the file and note the changes after `ls -ltr`
 	![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/34e6d70e-ae93-4a2c-b06a-79272d33857f)


2) Write an article about File Permissions based on your understanding from the notes.

3) Read about ACL and try out the commands `getfacl` and `setfacl`

In case of any doubts, post it on [Discord Community](https://discord.gg/hs3Pmc5F)

$ getfacl my_directory
# Output will show the ACL entries for the specified directory.

$ setfacl -m u:user1:rw my_file
# This grants read and write permissions to user1 on the specified file.


Happy Learning
