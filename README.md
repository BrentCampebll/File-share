# File-share
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>File Sharing in Active Directory (Azure)</h1>
This tutorial outlines the implementation of File sharing in Active Directory and permitting and denying access.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create Folders
- Assign access to folders
- Test access and permissions

<h2>Deployment and Configuration Steps</h2>

<p>
<img <a href="https://imgur.com/uCajK8p"><img src="https://i.imgur.com/uCajK8p.png" title="source: imgur.com" /></a>
<a href="https://imgur.com/52ZSzqe"><img src="https://i.imgur.com/52ZSzqe.png" title="source: imgur.com" /></a>

</p>
<p>
Continuing from the previous set up we will login to DC-1 as an jane, and the VM as one of the created users (late.qusow) on our domain which was created before(daintanets.com).  On the C drive of DC-1, we create 4 folders wth varying access.  Then set permissions for each folder, Read access will be read access for domain users., no access will be read/write access for admins only, write access for read/write access for domain users, and accounting will only be accessible to a security group we will create called accountants.  Last we will test the various access levels of said folders oon the VM with the users we created granted different permissions and across several accounts.  Giving late.qusow access to the acoounting folder.
</p>

<img <a href="https://imgur.com/NyUxWQQ"><img src="https://i.imgur.com/NyUxWQQ.png" title="source: imgur.com" /></a>
<a href="https://imgur.com/HGnIiUw"><img src="https://i.imgur.com/HGnIiUw.png" title="source: imgur.com" /></a>

<br />

