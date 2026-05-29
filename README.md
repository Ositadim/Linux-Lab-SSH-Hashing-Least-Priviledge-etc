**Project Overview** <br/>
These labs focus on practical Linux skills required in cybersecurity roles, including:
- Installing and managing software using APT
- Examining input and output in the Bash shell
- Navigating and managing the Linux filesystem
- Filtering and searching log data
- Creating and modifying files and directories
- Managing permissions, ownership, and users
- Applying the principle of least privilege
<br/>
<p><strong>**Linux File Recording**:</strong> <a href="https://drive.google.com/drive/folders/10l66EblVzahm8ITEd6dWs4Mu5Msj2hZW?usp=sharing" target="_blank" rel="noopener noreferrer">Open Google Drive folder</a></p>
<br/>
<p><strong>**Log Analysis Recording**:</strong> <a href="https://drive.google.com/drive/folders/1LEuEFPwyLwPDtSlDcxy4lxlzR5OIPVR4?usp=sharing" target="_blank" rel="noopener noreferrer">Open Google Drive folder</a></p>
<br/>
**Activity overview **
In this lab activity, you’ll use the Advanced Package Tool (APT) and sudo to install and uninstall applications in a Linux Bash shell. 
While installing Linux applications can be a complex task, the APT package manager manages most of this complexity for you and allows you to quickly and reliably manage the applications in a Linux environment. 
You'll use Suricata and tcpdump as an example. These are network security applications that can be used to capture and analyze network traffic. 
The virtual machine you access in this lab has a Debian-based distribution of Linux running, and that works with the APT package manager. Using a virtual machine prevents damage to a system in the event its tools are used improperly. It also gives you the ability to revert to a previous state. 
As a security analyst, it's likely you'll need to know how to install and manage applications on a Linux operating system. In this lab activity, you’ll learn how to do exactly that! 
**Scenario** 
Your role as a security analyst requires that you have the Suricata and tcpdump network security applications installed on your system. 
In this scenario, you have to install, uninstall, and reinstall these applications on your Linux Bash shell. You also need to confirm that you’ve installed them correctly. 
Here’s how you'll do this: First, you’ll confirm that APT is installed on your Linux Bash shell. Next, you’ll use APT to install the Suricata application and confirm that it is installed. Then, you’ll uninstall the Suricata application and confirm this as well. Next, you’ll install the tcpdump application and list the applications currently installed. Finally, you’ll reinstall the Suricata application and confirm that both applications are installed. 

**Lab practice 1**: on the use of apt package tool (Advanced Package Tool ); suricata and tcpdump installation and uninstalling. 
 **Using apt command **
- sudo apt install suricata suricata 
- sudo apt remove suricata 
- sudo apt install tcpdump tcpdump apt list –installed Output: 

  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/b63e7d21-b288-4b24-a431-ea25505bf216" />

  
# 
Video recording: https://screenrec.com/share/NkeE5ihLmR  
 
2. Activity: Examine input and output in the shell 
Introduction 
In this lab, you’ll use the 	echo	 command to examine how input is received and how 
output is returned in the shell. You’ll also use other Linux commands in the Bash shell to 
explore more about input and output and other basic functions of the shell 
What you’ll do 
You have multiple tasks in this lab: 
•	Generate output in the shell the echo command 
•	Perform basic calculations the expr command 
•	Clear the shell window the clear command 
•	Explore the commands further 
 
Lab practice 2:  on the Use of Bash

- echo osita echo “osita” expr 3 + 4 clear 
- Lab practice 3: Commands Used in Linus 
- Pwd – current working directory. The absolute file path. The whoami = username  
- Ls - list 
- Cd – change directory 
- cat (file name)– displays the content of a file head (file name) – content display by default 10 lines of the file 
 
Filesystem Hierarchy Standard 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/610023bd-f8fc-4a09-8967-405f5e90943d" />

  
	• 	A file path is the location of a file or directory 
	• **	root directory** - (/) 
  •	**/home**: Each user in the system gets their own home directory. 
  • **/bin:** This directory stands for “binary” and contains binary files and other executables.            Executables are files that contain a series of commands a computer needs to follow to run            programs and perform other functions. 
  •	**/etc**: This directory stores the system’s configuration files. 
  • **/tmp**: This directory stores many temporary files. The 	/tmp	 directory is commonly 
      used by attackers because anyone in the system can modify data in these files. 
  • **/mnt**: This directory stands for “mount” and stores media, such as USB drives and 
       hard drives. 
       

**Reading File Content:** cat	, 	head	, 	tail	, and 	less
**Cat:** entering cat updates.txt returns everything in the updates.txt file. 
**Head** : displays the content of the file 
if you only want to display the first five lines of the** updates.txt file**, enter **head -n 5 
updates.txt**
**tail: ** The 	tail	 command does the opposite of 	head	. This command can be used to 
display just the end of a file, by default 10 lines. Entering only the last 10 lines of the updates.txt file. 	
tail updates.txt
	 returns 

		
Pro Tip: You can use tail to read the most recent information in a log file. 
Less: The less command returns the content of a file one page at a time.  
Once you’ve accessed your content with the 	less	 command, you can use several 
keyboard controls to move through the file: 
•	Space bar: Move forward one page 
•	b: Move back one page 
•	Down arrow: Move forward one line 
•	Up arrow: Move back one line 
•	q: Quit and return to the previous terminal window 

**Lab Practice 4: **

**Activity overview **

Previously, you learned about Linux and how to communicate with the OS through the shell. You also learned how to use some of the core commands to navigate the Linux file system and read content from files it contains. 
These are essential skills. For example, when investigating unauthorized access, you might navigate to and then read a user access report. 
In this lab activity, you’ll navigate a Linux file structure, locate files, and read the contents of files. You’ll also need to answer a few multiple-choice questions based on the information contained in these files. 
As a security analyst, it’s key that you know how to navigate, manage, and analyze files remotely via a Linux shell without a graphical user interface. 
This exemplar is a walkthrough of the previous Qwiklab activity, including detailed instructions and solutions. You may use this exemplar if you were unable to complete the lab and/or you need extra guidance in competing lab tasks. You may also refer to this exemplar to prepare for the graded quiz in this module. 
Practice screenshot 
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/c6ec7b2c-a6c0-4ed1-a30e-76b6d6152dd6" />

 <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/f38ef45b-523f-4846-ba2d-7c0e52a18d67" />

 
**Filter content in Linux** 
 
Filtering is selecting data that match a certain condition. 
The **grep** command searches a specified file and returns all lines in the file containing a specified string or text. The grep command commonly takes two arguments: a specific string to search for and a specific file to search through. 
 	example: **grep error time_logs.txt** 
The pipe command is accessed using the pipe character (|). **Piping** sends the standard output of one command as standard input to another command for further processing.  
For example, ls /home/analyst/reports | grep users returns the file and directory names in the reports directory that contain users. Before the pipe, **ls** indicates to list the names of the files and directories in reports. Then, it sends this output to the command after the pipe.  
You can think of piping as a general tool that you can use whenever you want the output of one command to become the input of another command. 
 
**find** 
The find command searches for directories and files that meet specified criteria.  
When using 	find	, the first argument after 	find	 indicates where to start searching. For
example, entering 
projects
the 	 	
find /home/analyst/projects
	 searches for everything starting at
	directory.  	
Specifying criteria involves options. **Options** modify the behavior of a command and commonly begin with a hyphen (-).  
-name and -iname 
One key criteria analysts might use with find is to find file or directory names that contain a specific string. The specific string you’re searching for must be entered in quotes after the -name or -iname options. The difference between these two options is that -name is casesensitive, and -iname is not.  
**Note**: An **asterisk (*)** is used as a wildcard to represent zero or more unknown characters. 
**-mtime** 
**Security analysts** might also use find to find files or directories last modified within a certain time frame. The -mtime option can be used for this search. For example, entering find /home/analyst/projects -mtime -3 returns all files and directories in the projects directory that have been modified within the past three days.  
The **-mtime** option search is based on days, so entering **-mtime +1 **indicates all files or directories last modified more than one day ago, and entering -mtime -1 indicates all files or directories last modified less than one day ago.  
Note: The option **-mmin **can be used instead of -mtime if you want to base the search on minutes rather than days. 

**Lab Practice**
**Scenario**
In this scenario, you need to obtain information contained in server log and user data files. 
You also need to find files with specific names. 
Here’s how you’ll do this: First, you’ll navigate to the logs directory and return the error messages in the server_logs.txt file. Next, you’ll navigate to the users directory and search for files that contain a specific string in their names. Finally, you’ll search for information contained in user files. 
 
 
Solution: https://screenrec.com/share/J52VAg0ySB  
commands used:  
Task 1: Navigate to logs and find error messages 

_cd /home/analyst/logs grep error server_logs.txt _
 
# Task 2: Navigate to users reports and find files by name cd /home/analyst/reports/users ls | grep Q1 ls | grep access 
 
# Task 3: Search inside user files
ls 
grep jhill Q2_deleted_users.txt 
grep "Human Resources" Q4_added_users.txt 
  
 <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/349f6a4d-5fcf-4eb5-898a-78dcfbb2e6a6" />

**Create and modify directories and files **

**Mv** – file name into (specify the directory you want to move it to starting from the root) 
 
**rmdir** – remove directory. The rmdir command cannot delete directories with files or                      subdirectories inside. For example, entering rmdir /home/analyst returns an error message. 
**mkdir** – create a directory(name of directory) 
**touch** – creat a file(name and text format)
**rm** – file remove 
**cp** – copy file to a different directory (does not delete the original) 
**nano** – file editor. Nano (name of the file you want to edit) you have to be in the file you want to edit. 
**Ctrl O** – to save, enter to save with current user name. No autosaving.  Ctrl x – exit 
 
You can also create a new file in nano by entering _nano_ followed by a new file name. For example, entering nano authorized_users.txt from the 
/home/analyst/reports directory creates the authorized_users.txt file within that directory and opens it in a new nano editing window. 
**Note**: Vim and Emacs are also popular command-line text editors. 
la	 
_In addition to the pipe (|), you can also use the right angle bracket (>) and double right angle bracket (>>) operators to redirect standard output. 
When used with 	echo	, the 	> and 	>>	 operators can be used to send the output of 	echo	 to a
>>_
specified file rather than the screen. The difference between the two is that **>** overwrites your existing file, and 	 adds your content to the end of the existing file instead of overwriting it. The > operator should be used carefully, because it’s not easy to recover overwritten files. 
When you’re inside the directory containing the permissions.txt file, entering echo 
"last updated date" >> permissions.txt adds the string “last updated date” to the file contents. Entering echo "time" > permissions.txt after this command overwrites the entire file contents of permissions.txt with the string “time”. 
Note: Both the 	> 
your specified name.
and >> operators will create a new file if one doesn’t already exist with 
 
  
**Lab Activity: Manage files with Linux commands** 

cd /home/analyst mkdir
logs 
ls 
rmdir temp 
ls 
cd notes mv Q3patches.txt /home/analyst/reports/ ls
/home/analyst/reports rm tempnotes.txt 
ls 
touch tasks.txt 
ls 
nano tasks.txt 
clear cat 
tasks.txt 
 
 <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/036570a3-cd88-48b3-b6f1-df9f0a38651c" />

 <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/75d28327-5ac6-4fde-a274-843df7525eb7" />

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/3f099c6d-1acc-4852-a92c-d706868eba9d" />

File permissions and ownership 
Ls – list 
Ls -a = list hiddend files too 
Ls -la = permissions to files and directory, including hidden files 
Ls -l  = extended info on the file, permission and format. Displays permissions to files and directories. Also displays other additional information, including owner name, group, file size, and the time of last modification. 
	 
 
**Change permissions: for The principle of least privilege**

chmod = change mode  	symbolic: chmod g+w, o-r access.txt persmissions to who g group o other u user permition types w write r read x execute 
 
following command would add all permissions to login_sessions.txt: 
chmod u+rwx,g+rwx,o+rwx login_sessions.txt 
If you wanted to take all the permissions away, you could use 
chmod u-rwx,g-rwx,o-rwx login_sessions.txt 
Another way to assign these permissions is to use the equals sign (=) in this first argument. 
Using = with group, and other:	
chmod
	login_sessions.txt
 sets, or assigns, the permissions exactly as specified. For example, the following command would set read permissions for 	 for user, 
	 	
**Character and Description **
u 	indicates changes will be made to user permissions 
g 	indicates changes will be made to group permissions 
o 	indicates changes will be made to other permissions 
+ 	adds permissions to the user, group, or other 
- 	removes permissions from the user, group, or other 
= 	assigns permissions for the user, group, or other 
Note: When there are permission changes to more than one owner type, commas are	 
chmod u=r,g=r,o=r login_sessions.txt 
needed to separate changes for each owner type. You should not add spaces after those commas. 

**The principle of least privilege in action**
As a security analyst, you may encounter a situation like this one: There’s a file called bonuses.txt within a compensation directory. The owner of this file is a member of the Human Resources department with a username of hrrep1. It has been decided that hrrep1 needs access to this file. But, since this file contains confidential information, no one else in the hr group needs access. 
You run 	ls -l	 to check the permissions of files in the compensation directory and 
discover that the permissions for 	
bonuses.txt
	 are 	
-rw-rw----
	. The group owner type 
   
	has read and write permissions that do not align with the principle of least privilege.			
To remedy the situation, you input chmod g-rw bonuses.txt. Now, only the user who needs to access this file to carry out their job responsibilities can access this file. 
 
 
Lab practice: doc link: [Google Doc Link](https://docs.google.com/document/d/1_Q_kvpvsM3_3I_7wUoIm-hGY-Z-ubaTtlArWlz-0bqE/edit?usp=sharing) 
Code:  cd /home/researcher2/projects 
ls -l ls -la 
chmod o-w project_k.txt 
ls -l 
chmod g-r project_m.txt 
ls -la 
chmod u-w,g-w,g+r .project_x.txt 
ls -l 
chmod g-x drafts 
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/f83c879c-6fac-4621-a013-a4f6644cca26" />

   <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/c75782c5-d08e-4623-ae17-ca554ae98745" />

Add and delete users 
 
**Types of users** 
Root user – supper user. sudo provides control to root user access. Special privileges. 
Useradd = sudo useradd osita 
Userdel – sudo userdel osita 

• -g: Sets the user’s default group, also called their primary group 
• -G	: Adds the user to additional groups, also called supplemental or secondary groups 
To use the 	-g	 option, the primary group must be specified after 	-g	.

For example, entering sudo useradd -g security fgarcia
	 adds fgarcia as a new user and assigns their primary group to be security. 			
To use the **-G** option, the supplemental group must be passed into the command after -G. You can add more than one supplemental group at a time with the -G option. Entering sudo useradd -G finance,admin fgarcia adds fgarcia as a new user and adds them to the existing finance and admin groups. 
 
 

**Usermod** 
The usermod command modifies existing user accounts. The same -g and -G options from the useradd command can be used with usermod if a user already exists.  
To change the primary group of an existing user, you need the 	-g	 option. For example, 
entering group to the 	
sudo usermod -g executive fgarcia would change fgarcia’s primary executive group. 			
To add a supplemental group for an existing user, you need the 	-G	 option. You also need a 
-a option, which appends the user to an existing group and is only used with the -G option. For example, entering  _sudo usermod -a -G marketing fgarcia_ would  add the existing **fgarcia** user to the supplemental marketing group. 	
			
Note: When changing the supplemental group of an existing user, if you don't include the -a option, -G will replace any existing supplemental groups with the groups specified after usermod.  Using -a with -G ensures that the new groups are added but existing groups are not replaced. 
 
**Chown** 
There are other options you can use with usermod to specify how you want to modify the user, including: 
•	-d: Changes the user’s home directory. 
•	-l: Changes the user’s login name. 
•	-L: Locks the account so the user can’t log in. 
The userdel command deletes a user from the system.  
The chown command changes ownership of a file or directory. You can use chown to change user or group ownership. To change the user owner of the access.txt file to fgarcia, enter sudo chown fgarcia access.txt. To change the group owner of access.txt to security, enter sudo chown :security access.txt. You must enter a colon (:) before security to designate it as a group name. 
 
**Task**
sudo useradd researcher9
sudo usermod -g research_team researcher9 
sudo chown researcher9 /home/researcher2/projects/project_r.txt 
sudo usermod -a -G sales_team researcher9 
sudo userdel researcher9 
sudo groupdel researcher9 

   <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/db5d9ac4-acdd-4a37-ad03-e7d22afdf400" />

Resources: 
man = manual (man usermod) whatis = what a command does (eg: whatis tail_ 
apropos = -a or with key word for specificity. when you don’t know what to look up…. Eg: how to change password, use the word “password” output of the man command is also called a “man page.” 
   
 
**Practical Application in Lab**

codes whatis cat man cat 
apropos -a first part file 
man useradd whatis rm 
whatis rmdir 
apropos -a create new group 
 
 
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/ac0eeeca-7b6a-415f-b3ce-b20e3fd7812a" />

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/2ff45c3a-423f-456c-be0b-8ee5752c7f53" />



