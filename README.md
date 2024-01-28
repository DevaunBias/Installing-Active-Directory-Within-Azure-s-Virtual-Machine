 <h1><p align="center"> 
 INSTALLING ACTIVE DIRECTORY WITHIN AZURE'S VIRTUAL MACHINE
 </p><h1>


<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

 
 [YouTube Demonstration](https://youtu.be/DDd8cXXhgTQ)
 

<h2>Description</h2>
Project consists of using Microsoft's cloud platform Azure. To create a Virtual Machine that will be running Windows Server 2022. With this Virtual Machine, we will be able to install Active Directory and make it a Domain Controller. The steps are very easy to understand and simple. You will only need either a paid or free account with Azure.
<br />


<h2>Languages and Utilities Used</h2>

- <b>None</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)
- <b>Windows Server 2022</b> (x64 Gen2)
- <b>Azure Virtual Machine</b>
- <b>Remote Desktop</b>
- <b>Active Directory Domain Services</b> 

<h2>Installation walk-through:</h2>

<p align="center">
Login to you Azure account and proceed to the Virtual Machine tab: <br/>
<img src="https://i.imgur.com/1rdUcB1.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select Create in the menu bar:  <br/>
<img src="https://i.imgur.com/xHP846z.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Fill out the "Project Details": <br/>
<img src="https://i.imgur.com/eLf424d.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select which image the Virtual Machine will be running:  <br/>
<img src="https://i.imgur.com/thYOeyW.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select your username and password for the account:  <br/>
<img src="https://i.imgur.com/iPCjbkp.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select Review + Create at the bottom left:  <br/>
<img src="https://i.imgur.com/WrKqUCm.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once Validation has passed, select Create:  <br/>
<img src="https://i.imgur.com/oQq2RKv.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete, select the newly made Virtual Machine and copy it's public IP Address:  <br/>
<img src="https://i.imgur.com/jSvHBNF.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Navigate to the Remote Desktop Application by typing it in the Windows Search Bar. Paste the IP Address in the computer slot:  <br/>
<img src="https://i.imgur.com/AqpO9rN.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Enter the Username and Password you created for the Virtual Machine:  <br/>
<img src="https://i.imgur.com/3flwwW8.jp" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Wait while the Virtual Machine sets up, Once finished loading Windows Server will appear. Select Add Roles & Features:  <br/>
<img src="https://i.imgur.com/XV5gOKq.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Press Next on the installation guide until you reach select server roles. Here is where you'll click Active Directory Domain Services:  <br/>
<img src="https://i.imgur.com/aigUC97.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Confirm settings are correct and install:  <br/>
<img src="https://i.imgur.com/rLN4RsJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Let Active Directory finish installing. Windows Server should appear like this. Click the caution logo, top right of the application:  <br/>
<img src="https://i.imgur.com/nzP2OqY.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 To finish Active Directory, we must promote it to a domain server:  <br/>
<img src="https://i.imgur.com/XSCsAa8.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Add a new forrest and give the server a domain name. I used mydomain.com:  <br/>
<img src="https://i.imgur.com/M7xzwSu.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Continue by pressing next and then install:  <br/>
<img src="https://i.imgur.com/xHioQIz.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 When the process is finished, the Virtual Machine will restart. You will have to reconnect, the username will now be the domain name you've chosen, backslash the original username from before:  <br/>
<img src="https://i.imgur.com/wwFHheL.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 The Virtual Machine and Windows Server will load again. You can now go to Tools > Active Directory Users and Computers:  <br/>
<img src="https://i.imgur.com/xPOQQ2o.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Active Directory is complete. Configure, test out any features you want:  <br/>
<img src="https://i.imgur.com/I4DOkLI.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
