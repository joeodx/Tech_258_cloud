# Linux Command Reference
************************************************************
![LINUX](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbiV23uy6NDy1C85mVlwH4HXgWz4ebcwCYwqgzS3PvIQ&s)

# Basic Linux Commands
*************************
## 'exit'

* Used to exit the current shell 

```python
exit
```
## 'clear'

* Used to clear terminal screen

```python
clear
```
## 'ls'

* Lists directory contents.

```python
ls [options] [file|directory]
```
## 'cd'

* Changes the current directory.

```python
cd [directory]
```
## 'history'

* Displays a list of the previous commands typed 

```python
history
```


## 'mkdir'

* Creates a new directory 

````python
mkdir [directory_name]
````
##  'cp'

* Copies files and directories.

```python
cp [source] [destination]
```
##  'rm - r'

* Removes files or directories.

```python
rm -r [directory]
```

##  'curl'

* Transfers data from or to a server, supporting various protocols including HTTP, HTTPS, FTP, etc. 

````python
curl [options] [URL]

````

## 'mv'

* Moves a file or renames it.

```python
mv [filename]
```

##  'touch'

* Creates an empty file.

````python
touch [filename]
````

## 'nano'

* Opens a file in the Nano text editor for editing.

```python
nano [filename]
```

##  'cat'

* Displays the contents of a file.

````python
cat [filename]
````

##  'head'

* Prints the top lines of a file.

```python
head -n [number_of_lines] [filename]
```

## 'tail'

* Prints the last lines of a file

````python
tail -n [number_of_lines] [filename]
````
<br>
<br>


# Commands to navigate and interacting with directories 
*************************************

## 'ls' 

*  lists files and directories in the current directory.
````python
ls 
````

## 'ls -a and ls -la'

* This command lists all files including hidden
```python
ls -a 
```
* This command lists all files and directories showing their permissions

```python
ls -la
```
## 'pwd'
* Shows current working directory 
```python 
pwd
```
<br>
<br>

# Commands to interact, update, install packages and automate in linux...
*************************************

## 'sudo apt update'

* Updates current packages
```python
sudo apt update -y
```

## 'sudo install'

* Install packages e.g like tree 

````python
sudo snap install tree
````

* what is tree? 

tree allows you to see a diagram of your files and directories : 

![](https://i.stack.imgur.com/VZxA1.png)

## 'Upgrade, install, restart and enable nginx'
* Upgrade nginx
```python
sudo apt update nginx -y --with-new-pkgs
```
* Install nginx
```python
sudo apt install nginx -y --with-new-pkgs
```

* The --with-new-pkgs flag allows the upgrade/installation to proceed even if there are new package dependencies (like a new kernel) that require a system restart. This should prevent the script from getting stuck at the kernel upgrade prompt.

<br>

* Restart nginx
```python
sudo systemctl restart nginx
```
* Enable nginx
```python
sudo systemctl enable nginx
```
* What is nginx?

Nginx (pronounced "engine-x") is a popular open-source web server and reverse proxy server software. Originally developed by Igor Sysoev in 2004, Nginx is known for its high performance, stability, and low resource consumption, making it a preferred choice for serving web content, handling high-traffic websites, and acting as a reverse proxy for various applications.

![](https://miro.medium.com/v2/resize:fit:1200/0*mjG1YdoT7xPcnznN.jpg)

<br>
<br>

# Linux permission forms 
*********************************

* Linux permissions are a system of access control that regulate who can read, write, or execute files and directories. Each file and directory is associated with three sets of permissions: one for the owner of the file, one for the group the file belongs to, and one for everyone else. These permissions are represented by three characters each, indicating whether the respective user or group has read ('r'), write ('w'), or execute ('x') permissions. By setting these permissions appropriately, Linux administrators can restrict or grant access to files and directories, ensuring data security and integrity within the system. Additionally, permissions can be further refined using special modes such as the setuid, setgid, and sticky bit to control file execution and inheritance of group ownership.

Long form, as letters (rw-r--r--) short form, as numbers (777)
https://chmod-calculator.com/

# Environmental variables commands
**********************************

* Shows the environmental variables 

```python
printenv
```

