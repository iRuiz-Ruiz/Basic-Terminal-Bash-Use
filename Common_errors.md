# How to install WSL (Ubuntu) in Windows 11?
Follow this [tutorial](https://www.youtube.com/watch?v=Re4WMV2Flvo)

# How to install WSL (Ubutu) in Windows 10?
Follow this [tutorial](https://www.youtube.com/watch?v=UsJTAbvM_ls)

# Change from root to your user 

Main cause: 
* You closed your WSL / Ubuntu windows before defining your user.

It might look like this 
```
root@YOURMACHINENAME windows/path/file
```
Solution:

**EASIEST**

Uninstall UBUNTU and Install it again, making sure you set your username and password correctly. 

**ALTERNATIVE (PRO VERSION)**

To solve this problem, you will need to know your password, if not, you could recover your password from this tutorial. 

1. Create new user name
```
adduser YOURUSERNAME
```
2. Give write and edit permissions to your username
```
sudo usermod -aG sudo YOURUSERNAME
```

3. Change from root to your username
```
su - YOURUSERNAME
```

In case you want to return to root and create new users:
```
sudo su
```

It should be ready to use and look like this in the Ubuntu window:
```
YOURUSERNAME@YOURMACHINE
```
# Unistall Ubuntu 
### Why am I unstalling Ubuntu?
Lately, I've been experiencing issues with the latest versions of Ubuntu, as they keep crashing onn the Visual Studio Code. It literally keeps stuck. 
However, it might be due to as well due to connection lost with the remote machine I'm trying to connect as it keeps happening with the v20.04.

### Steps
1. Unistall Ubuntu as a regular program.
2. Go to powershell and delete the Ubuntu branch you are using.
```
wsl --help ## this command will show which options you can access from WSL
wsl --list ## list the versions of the installed Ubuntu
wsl --unregister <Distros or Ubuntu version> ## this command delete the Ubuntu version you are interested to delete
```
3. Go to this path, and delete the associated files. 
```
C:\Users\isabe\AppData\Local\Packages

## AppData is a hidden folder which can be only accessed from the path.

## The associated files will start with CanonicalGroupLimited.Ubuntu2x.0x
```
4. Deactivate the Windows Subsystem for Linux Optional Feature (Settings>Systems>Optional Features) and restart.

A step by step tutorial is available at ZacsTech (see link below). 

# References
IONOS [https://www.ionos.co.uk/help/server-cloud-infrastructure/server-administration/creating-a-sudo-enabled-user/]
UNIX & LINUX [https://unix.stackexchange.com/questions/156962/how-to-change-to-normal-user-in-the-command-line-when-logged-in-as-the-root-user]
1Gbits [https://1gbits.com/blog/how-to-switch-to-root-user-ubuntu/]

Thank to Gazal

To delete Ubuntu
Mastering WSL [https://locall.host/wsl-uninstall-ubuntu/#google_vignette]
ZacsTech [https://www.youtube.com/watch?v=boFhEF8eSxg]
