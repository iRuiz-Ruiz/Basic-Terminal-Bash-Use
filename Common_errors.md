# How to install WSL (Ubuntu) in Windows 11?
Follow this [tutorial](https://www.youtube.com/watch?v=Re4WMV2Flvo)

# How to install WSL (Ubutu) in Windows 10?
Follow this [tutorial](https://www.youtube.com/watch?v=UsJTAbvM_ls)

# Common problems

## Why am I in root?

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

It should be ready to use and look like this in the Ubuntu window:
```
YOURUSERNAME@YOURMACHINE
```

# References
IONOS [https://www.ionos.co.uk/help/server-cloud-infrastructure/server-administration/creating-a-sudo-enabled-user/]
UNIX & LINUX [https://unix.stackexchange.com/questions/156962/how-to-change-to-normal-user-in-the-command-line-when-logged-in-as-the-root-user]

Thank to gazal
