<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://imgur.com/rLfJdhf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First step after getting a Windows Server virtual machine up and running it is important to set the IP adress to Static.
</p>
<br />

<p>
<img src="https://imgur.com/MlvYdm6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy the public IP Address and using Remote Desktop Connection connect to the Windows Server.
</p>
<br />

<p>
<img src="https://imgur.com/f6BlIFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When Windows Server boots up server manager should open. To begin installing Active Directory click Add roles and features.
</p>
<br />

<p>
<img src="https://imgur.com/OhrrADC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you get to this screen make sure to select "Active Directory Domain Services" 
</p>
<br />

<p>
<img src="https://imgur.com/UnKoOSc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Installation finishes click on the notification flag and select promote this server to a domain controller.
</p>
<br />

<p>
<img src="https://imgur.com/TgIkcQr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this screen select Add a new forest and choose a name for the domain server ex: mydomain.com click next and install.<br>
Finally the Server will require a restart. 
</p>
<br />

<p>
<img src="https://imgur.com/0VTnf8t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You will now need to log in with the context of the domain ex: mydomain.com\labuser
</p>
<br />
