# VMWarePro-Active
Transitioning my existing Active Directory Homelab environment (using Virtualbox) to Vmware for a more practical applications. 
Much like my previous homelab environment using Virtualbox, we will be using the following: 
- A Windows Server ISO
- A Windows Client ISO
- VMWare Workstation
# Installing Windows Server 
Using the VMware Workstation wizard, we will be installing Windows Server to host Active Directory. 
<img width="1229" height="1015" alt="image" src="https://github.com/user-attachments/assets/c023cca8-f6db-4138-9afe-ddf9eff08c5a" />
The wizard will prompt you to add the Windows Server ISO for install.
Note that you will be prompted to provide a Windows product key. Although it is preferred, for our use, we do not need the product key at this time. You may also enter a password for login, otherwise just click "next". 

<img width="616" height="511" alt="Screenshot 2025-12-08 224925" src="https://github.com/user-attachments/assets/73966581-a127-447e-a02d-8880d2a6da8a" />

Next, name your VM and choose the location you would like to save the files. 
<img width="1233" height="1021" alt="image" src="https://github.com/user-attachments/assets/5b69c679-3898-4f07-b1be-f3eb329b2c55" />

Choose your desired disk size, for the sake of time and continuety, I will be using the default 60GB allocation and splitting the virtual disk into multiple files to improve performance. 
<img width="1227" height="1019" alt="image" src="https://github.com/user-attachments/assets/ce61bcb5-b437-4d45-8f00-24584cc2394a" />

Lastly, ensure you uncheck the "Power on this virtual machine after creation" to avoid getting errors during installation. Click Finish. 

<img width="614" height="511" alt="Screenshot 2025-12-08 225849" src="https://github.com/user-attachments/assets/2af7d768-a314-4ff7-b74e-7eaf603d62ce" />

Before install, we will be removing the floppy disk to prevent any errors during installation. This is done by editing the virtuam machine settings in VMWAre Workstation. 

<img width="613" height="508" alt="Screenshot 2025-12-08 230007" src="https://github.com/user-attachments/assets/3456b796-0921-4771-9525-1d42065c7e51" />
<img width="740" height="533" alt="image" src="https://github.com/user-attachments/assets/e35eb050-b61e-4314-b6ff-fd305696c34f" />
Now, we power on the Virtual MAchine and go through the install prompts. Being sure to choose the Operating System that includes the "Desktop Experience". If not, you will be running a server strictly through command line. 
<img width="1230" height="944" alt="image" src="https://github.com/user-attachments/assets/9163956a-f811-4dff-a925-4cb18103426f" />
You will be prompted to input your passowrd and then click "Finish" to complete the installation. 
<img width="1223" height="1020" alt="image" src="https://github.com/user-attachments/assets/26a936b1-0dd5-44ae-be5c-8716eec1b039" />

After install, you will be met with the login screen. Login using your password. From there, you should be met with Server Manager. 
<img width="1252" height="944" alt="image" src="https://github.com/user-attachments/assets/f7f3fe4f-89cc-4210-b2ba-e4a40fcdce41" />
# Renaming the VM using Server Manager 
With many ways to do this, utilizing the Server Mananger seems to be one of easiest and most straight forward. Click Local Server > The hyperlink for the computer. This will bring up a window that will allow you to change the name as you see fit. 
<img width="1231" height="943" alt="image" src="https://github.com/user-attachments/assets/9a520e02-f37a-4c31-99d1-17055d01499b" />
<img width="616" height="470" alt="image" src="https://github.com/user-attachments/assets/7a4d57a7-09c9-44d9-9e00-82bbfadcf09f" />
<img width="1231" height="938" alt="image" src="https://github.com/user-attachments/assets/da41a747-d3bb-4f71-957a-0d00aa323339" />
Once it has been renamed, Windows will restart. 
# Configure Static IP Address 




