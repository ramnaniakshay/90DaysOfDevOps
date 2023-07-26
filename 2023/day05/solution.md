Task 1: If you noticed that there are total 90 sub directories in the directory '2023' of this repository. What did you think, how did I create 90 directories. Manually one by one or using a script, or a command ?

All 90 directories within seconds using a simple command.

 mkdir day{1..90}

Tasks
You have to do the same using Shell Script i.e using either Loops or command with start day and end day variables using arguments

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/e52ad45e-e632-4460-b2db-9f9cb6301979)

make sure you provide permission to execute this file.

I used "chmod 700 filename"

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/cb56f4aa-0f92-4ca4-a016-4f0f8ab79899)

Task 2: Create a Script to backup all your work done till now.

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/0a21ed65-ff99-48f6-b60b-2b4927ad8206)

make sure you provide permission to execute this file.

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/ef792fef-dfa6-4983-b10c-d9998aaaadd1)

Task 3: Read About Cron and Crontab, to automate the backup Script

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/1ea93e4b-d92e-4d19-b712-bedb8dfab4b8)

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/9617d423-688e-47f9-9d0b-2193964832e8)

Task 4: Read about User Management and Let me know on Linkedin if you're ready for Day 6.

User management in Linux refers to the process of creating, modifying, and managing user accounts and permissions on a Linux system. It is an essential aspect of system administration and plays a crucial role in maintaining the security, access control, and overall stability of the Linux environment. From a DevOps point of view, user management is important for several reasons:

->Access Control: In a DevOps environment, multiple team members collaborate on various projects. User management allows administrators to grant appropriate access privileges to team members, ensuring that each user has the necessary permissions to perform their tasks without compromising security.

->Security: Proper user management helps enforce the principle of least privilege, where users only have access to the resources they require for their roles. By setting up user accounts with the right permissions, the risk of unauthorized access to critical system files and data is reduced.

->Auditing and Accountability: User management enables tracking user activities and actions on the system. It helps identify who performed specific actions, making it easier to troubleshoot issues, investigate security breaches, and maintain accountability within the DevOps team.

->Isolation: Creating separate user accounts for different users helps isolate their processes and activities from each other. This isolation ensures that one user's actions or errors do not adversely affect others or the system as a whole.

->Automated Deployments: In DevOps, automation plays a significant role in deploying applications and managing infrastructure. Proper user management allows DevOps tools and scripts to authenticate and execute actions securely without compromising sensitive data.

->Configuration Management: Configuration management tools, such as Ansible, Chef, or Puppet, often rely on specific user accounts for managing configurations across multiple servers. Properly configuring user accounts ensures that these tools can carry out their tasks effectively.

->Continuous Integration and Continuous Deployment (CI/CD): In CI/CD pipelines, user management is crucial for granting access to various deployment environments and tools used in the automation process.

->Disaster Recovery: User management also plays a role in disaster recovery scenarios. Properly managing user accounts helps in restoring services and data access during recovery processes.


