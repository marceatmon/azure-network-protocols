<p align="center">
<img src="https://github.com/marceatmon/AD-files/blob/main/Active%20DirectoryLogo3.png" alt="osTicket logo"/>
</p>

<h1>Active Directory: Configuring Active Directory within Azure VMs</h1>
This tutorial outlines creating Domain Admins and Users in Active Directory.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Configuration</h2>

- Create an Admin and Normal User Account in AD
- Join Client-1 to your domain
- Setup Remote Desktop for non-administrative users on Client-1
- Create additional users and attempt to login Client-1 with one of the users

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/marceatmon/AD-files/blob/main/Creating%20New%20Active%20Directory%20User.jpg?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
In Active Directory, new Employees, Admins, and Security Groups can be created. Right click on your domain name and click on Organizational Unit to create new folders. After the Admins and Employees folders have been created, create an Admin user for the Admin folder. Right click on the _ADMINS folder under your domain and click on User.

</p>
<br />

<p>
<img src="https://github.com/marceatmon/AD-files/blob/main/Adding%20User%20to%20Security%20Group.jpg?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the user has been created, the account must be added as an Admin to that folder. To add this user as an Administrator right click on the name and click on Properties. Click on the Member Of tab and double click on Domain Users to open the next window.
</p>
<br />

<p>
<img src="https://github.com/marceatmon/AD-files/blob/main/Setting%20Client-1's%20DNS%20settings%20to%20DC-1's%20Private%20IP%20address.jpg?raw=true" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the group box is populated, type "domains" in enter the object names to be selected box-->Click on Check Names to the right-->Select Domain Admins-->Click Ok-->Click on Apply-->Click Ok. This will add your user as a domain admin to your active directory. Log out of the server and log back into the server as the admin.
Once the group box is populated, type "domains" enter the object names to be selected box-->Click on Check Names to the right-->Select Domain Admins-->Click Ok-->Click on Apply-->Click Ok. This will add your user as a domain admin to your active directory. Log out of the server and log back into the server as the admin.
</p>
<br />
