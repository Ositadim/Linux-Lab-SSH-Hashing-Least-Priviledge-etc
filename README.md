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
**Lab 1****: Install Software in a Linux Distribution**
Objective: Use the Advanced Package Tool (APT) and sudo to install, uninstall, and verify network security tools in a Debian-based Linux environment.

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/0b9b3afe-ad5e-4754-a2da-5b67cd08ca28" />

Tools installed: 
Suricata – Network threat detection and intrusion detection system
tcpdump – Network packet capture and traffic analysis tool

- Confirm APT Availability:

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/913c9324-11c9-43eb-8acf-dd3695d7aa75" />

- Install Suricata

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/4af00e0e-c876-4ba3-bd08-7ffda561f5ce" />

- Uninstall Suricata <br/>
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/dd1c25f3-feb5-4a5e-a106-c167a12c083b" />

- Install tcpdump

  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/3204aa64-64ea-45aa-a29a-f6a7a2e6dc1f" />

- List Installed Applications
  
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/cd315cf7-c319-4d73-aa53-a70ec18e4475" />

- Expected output includes:

  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/f379f324-baad-4914-aaef-cfdba80a7d10" /><br/>
- 🎥 Video Recording:<br/>
<p><strong>Video recording:</strong> <a href="https://screenrec.com/share/NkeE5ihLmR" target="_blank" rel="noopener noreferrer">Watch here</a></p>

**Lab 2**: **Examine Input and Output in the Shell**
- **Objective**: Understand how input is received and output is returned in the Bash shell.
- Generate Output <br/>
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/502b0c67-00a0-4df3-8e43-a0a6ed9992a1" /> <br/>
- Perform Basic Calculations <br/>
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/ac6173a7-9cc8-41dd-ae86-af5d8e210d56" /><br/>
- Clear the Terminal <br/>
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/754951c4-af97-446e-9da0-2cbf40cf2400" />

**Lab 3: Core Linux Commands**
Common Commands Used

Command	    Description
pwd	        Displays current working directory
whoami	    Displays current user
ls	        Lists directory contents
cd	        Changes directory
cat	        Displays file contents
head	      Displays first 10 lines of a file

**Linux Filesystem Hierarchy Standard (FHS)**
Key directories explored in this lab:

/     – Root directory
/home – User home directories
/bin  – Executable binaries
/etc  – System configuration files
/tmp  – Temporary files (commonly targeted by attackers)
/mnt  – Mounted storage devices

**Useful Notes**
~ represents the user’s home directory
. represents the current directory
.. represents the parent directory
Absolute paths begin at /
Relative paths depend on the current directory

**Reading File Content**
Commands Used

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/78251f2c-7e66-4868-b806-cc92d655d5ff" />

**Navigation inside less:**
Space → forward one page
b → back one page
Arrow keys → line-by-line navigation
q → quit

**Lab 4: Navigate and Analyze Files**
Objective: Navigate Linux file structures, locate files, and analyze file contents without a graphical interface.

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/41cd2aaf-dcf3-47e1-8760-bef73f42514b" /> <br/>

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/86dcddec-6f63-4ecd-a686-4a4386a8f443" /> <br/>

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/2eb3a966-a9aa-4276-8772-391c938a8c8c" /> <br/>

**Filtering Content in Linux**
🔹 Search Text with grep <br/>
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/4e608a34-2aea-453a-a397-d39e8ef94914" />

- Pipe Output Between Commands <br/>
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/77b18434-7dd9-4282-8640-2a8c29e270b5" />

- Locate Files with **find**
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/74390dbe-8174-415a-b618-d441941b72ec" />

- Practical Tasks

  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/cafde8bb-ce8e-465d-a843-f7f7862985a2" />

- Create and Modify Files & Directories
  Commands Used

  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/a709b80c-ad23-49fd-9244-9c98cbcf2fe3" />

- Nano editor shortcuts:
  Ctrl + O → save
  Ctrl + X → exit

- File Permissions & Ownership
  View Permissions
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/44778c75-c9d9-4542-adc4-35cb59ce3c0e" />

- Modify Permissions with chmod. These commands demonstrate enforcement of the principle of least privilege.
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/3ea455a4-f4d6-45c0-90b5-caa26be35665" />

- User and Group Management
    - Add and Delete Users <br/>
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/fcfe5070-8ba9-409f-80ea-170c85d0e638" />
  
- Modify Existing Users
  
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/158d788d-e1ee-488e-adf2-40d71ef3cf03" />

- Change File Ownership
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/79827d26-5d19-498f-a086-b51f140e6aca" />

- Clean-Up Tasks
  
  <img width="333" height="71" alt="image" src="https://github.com/user-attachments/assets/3509b0f0-6271-4ee5-8f1d-1284995dd9af" />

**Linux Help & Documentation**

<img width="515" height="105" alt="image" src="https://github.com/user-attachments/assets/05d8efc1-59da-4b4c-a00d-da10627af269" />

