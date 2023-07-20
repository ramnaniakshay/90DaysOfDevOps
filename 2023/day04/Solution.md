Task solutions
 - Explain in your own words and examples, what is Shell Scripting for DevOps.

Shell scripting is like having linux commands all together in one file and once you execute all the commands will be also executed.
its like automating your linux machine.

example : 

you want to create a directory, and there you want to create one file , want to add fruits name in this file, want to print content of fruits file.

now if you create one shell script file which has all this commands written.

sample shell script which will perform above tasks

#--------------starting shell script file------------------------
mkdir demo
cd demo
cat << EOF > fruits.txt
Mango
Watermelon
Kiwi
Apple
EOF

cat fruits.txt
#---------------End of shell script file---------------------------


 - What is `#!/bin/bash?` can we write `#!/bin/sh` as well?
The line #!/bin/bash is called a "shebang" (also known as a hashbang),
and it is used to specify the interpreter that should be used to execute the script.
In this case, #!/bin/bash indicates that the script should be interpreted and executed using the Bash shell.

Yes, we can also use #!/bin/sh as the shebang to indicate that the script should be executed using the system's 
default shell (commonly, this points to the Bourne shell or a compatible shell). 
This is a more generic approach since /bin/sh typically points to the default shell on Unix-like systems, 
which could be Bash, Dash, Ash, or another compatible shell.
 
 - Write a Shell Script which prints `I will complete #90DaysOofDevOps challenge`
![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/774faa4c-0de0-47da-aa64-f5e4545d1b4f)

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/f58c89a6-dd95-48cd-8bbb-29ed15ed2f9e)

 - Write a Shell Script to take user input, input from arguments and print the variables.
![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/797260ee-c7e1-48d2-8120-eb2b24281175)

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/a12b3c53-1a29-4601-ac50-7d0b22fc7c3c)

 - Write an Example of If else in Shell Scripting by comparing 2 numbers
![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/15044b5c-da79-4e79-bfae-003efa35b1ab)

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/c28a1e16-151b-48ab-bb65-57754f7c3eb5)


