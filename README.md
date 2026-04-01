<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

1) Open Server Manager → Add Roles and Features
2) After Installation → Promote Server to Domain Controller
3) Set Directory Services Restore Mode Password (DSRM)
4) Complete Prerequisite Check → Install
5) Open Active Directory Users and Computers

<h2>Deployment and Configuration Steps</h2>

<p>
<h1>Open Server Manager → Add Roles and Features</h1>
<img width="796" height="564" alt="image" src="https://github.com/user-attachments/assets/8a980c03-3581-4c2e-884d-f136f904e224" />
<img width="800" height="567" alt="image" src="https://github.com/user-attachments/assets/848efc66-5709-46c5-8e32-c3f7c0dd9439" />
</p>
<p>
1.) Select Active Directory Domain Services
2.) Click Add Features
3.) Continue to Install
</p>
<br />

<p>
2) After Installation → Promote Server to Domain Controller
<img width="778" height="526" alt="image" src="https://github.com/user-attachments/assets/b7c66e52-935d-40a1-b09a-979d3c30892b" />
<img width="927" height="628" alt="image" src="https://github.com/user-attachments/assets/b75d02ed-ba6b-47b5-9da0-4de4cfb2e5d2" />
</p>
<p>
1.) Add a new forest
</p>
<br />

<p>
3) Set Directory Services Restore Mode Password (DSRM)
During promotion you must create a recovery password.

This password is used if AD needs emergency recovery.

⚠️ Save it carefully.
</p>
<p>
4) Complete Prerequisite Check → Install
<p>
<img width="389" height="155" alt="image" src="https://github.com/user-attachments/assets/8b1e8c3d-5477-4a1a-93e6-e3968d1b2a62" />
</p>
<br />

<p>
<h1>5) Open Active Directory Users and Computers</h1>
<img width="604" height="516" alt="image" src="https://github.com/user-attachments/assets/3e0f2ae4-3789-486b-bcb9-a35259eb1552" />
<img width="676" height="468" alt="image" src="https://github.com/user-attachments/assets/2fb77b9e-2b8e-496f-a2c2-d4db3602f845" />
</p>
<p>
Here you create:

-Users
-Groups
-Organizational Units (OUs)
</p>
<br />

<p>
<h1>1.)Open Active Directory Users and Computers></h1>
<img width="541" height="403" alt="image" src="https://github.com/user-attachments/assets/bec3dd91-888d-4447-aa0a-ab30e8341bfe" />
<img width="796" height="564" alt="image" src="https://github.com/user-attachments/assets/4c53b2db-ddfb-462c-b949-0bd70195f2bf" />
</p>
<p>
Go to:

Server Manager → Tools → Active Directory Users and Computers

You’ll see the domain tree on the left.
</p>
<br />

<p>
<h1>2)Choose the OU Where You Want the User</h1>
Example:

Right-click IT or Users

Then:

New → User

This opens the New User wizard.
</p>
<p>

<p>
<h1>3) Fill in User Information</h1>
<img width="775" height="566" alt="image" src="https://github.com/user-attachments/assets/c357120b-c46c-41f3-91b1-b110e2d293e0" />
<img width="773" height="569" alt="image" src="https://github.com/user-attachments/assets/c3ef1d51-3c1f-4593-b13c-360c94b0f99a" />
<p>
Enter:

First name: John
Last name: Smith
User logon name: jsmith
</p>
<br />

<p>
<h1>4) Set Password</h1>
Choose a temporary password like: temporary 123
Then check:
User must change password at next logon. 
<p>
<br />








