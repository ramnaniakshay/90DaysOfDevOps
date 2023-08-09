# Day 7 Task: Understanding package manager and systemctl

### What is a package manager in Linux?
 
 In simpler words, a package manager is a tool that allows users to install, remove, upgrade, configure and manage software packages on an operating system. The package manager can be a graphical application like a software center or a command line tool like apt-get or pacman.

 You’ll often find me using the term ‘package’ in tutorials and articles, To understand package manager, you must understand what a package is.

### What is a package?
 
 A package is usually referred to an application but it could be a GUI application, command line tool or a software library (required by other software programs). A package is essentially an archive file containing the binary executable, configuration file and sometimes information about the dependencies.

### Different kinds of package managers
 Package Managers differ based on packaging system but same packaging system may have more than one package manager.

 For example, RPM has Yum and DNF package managers. For DEB, you have apt-get, aptitude command line based package managers.


## Tasks

 1) You have to install docker and jenkins in your system from your terminal using package managers
install docker
    2  sudo apt-get update
    3  sudo apt-get install ca-certificates curl gnupg
    4  sudo install -m 0755 -d /etc/apt/keyrings
    5  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
    6  sudo chmod a+r /etc/apt/keyrings/docker.gpg
    7  echo   "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" |   sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    8  sudo apt-get update
    9  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   10  docker --version
   11  sudo apt update
   12  sudo apt install openjdk-17-jre
   13  java -version
   14  curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
   15  echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]   https://pkg.jenkins.io/debian-stable binary/ | sudo tee   /etc/apt/sources.list.d/jenkins.list > /dev/null
   16  sudo apt-get update
   17  sudo apt-get install jenkins
   18  jenkins --version


 2) Write a small blog or article to install these tools using package managers on Ubuntu and CentOS


### systemctl and systemd

 systemctl is used to examine and control the state of “systemd” system and service manager. systemd is system and service manager for Unix like operating systems(most of the distributions, not all).


## Tasks

 1) check the status of docker service in your system (make sure you completed above tasks, else docker won't be installed)
sudo systemctl status docker

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/fd15ed52-78d4-4322-8d0f-a8a31efc570d)


 2) stop the service jenkins and post before and after screenshots

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/dde08119-04c3-4aae-8b69-4ea365522bfc)


sudo systemctl stop jenkins

![image](https://github.com/ramnaniakshay/90DaysOfDevOps/assets/60702445/c8c7b8f5-805f-4800-bdd5-19811d402581)


 3) read about the commands systemctl vs service

 eg. `systemctl status docker` vs `service docker status`

 so systemctl is great and it has more features whereas service command was used in legacy systems and from my point of view systemctl is great as it holds more features compare to service

 basically this two commands are useful for start,stop,status or pause of application.

For Reference, read [this](https://www.howtogeek.com/devops/how-to-check-if-the-docker-daemon-or-a-container-is-running/#:~:text=Checking%20With%20Systemctl&text=Check%20what%27s%20displayed%20under%20%E2%80%9CActive,running%20sudo%20systemctl%20start%20docker%20.)


#### Post about this and bring your friends to this #90DaysOfDevOps challenge.

