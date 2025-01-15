<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post Installation Setup</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: Post Installation Configuration of OS Ticket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol (RDP)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post Installation Configuration Objectives</h2>

- Configure Roles, Departments, Teams, and Agents
- Enable open ticket creation for users
- Set up Users (Customers), SLA Policies, and Help Topics

<h2>Configuration Steps</h2>

### 1. Configure Roles for Grouping Permissions
<p>
<img src="https://github.com/user-attachments/assets/d111dfcc-3503-4118-ab4b-9c1b7f2f95d6" height="80%" width="80%" alt="Admin Agent Role Config"/>
</p>
<p>
  
Login to the ADMIN USER you created in part 1 where we setup osTicket. 

Navigate to Admin Panel → Agents → Roles.
  
Create a "Supreme Admin" role with full access.

</p>
<br />

### 2. Configure Department for SysAdmins
<p>
<img src="https://github.com/user-attachments/assets/2b463ca8-45c5-4acc-bda5-ba73408352d3" height="80%" width="80%" alt="Configure Department"/>
</p>
<p>
  
Navigate to Admin Panel → Agents → Departments.
  
Add a new department named SysAdmins and set it as a Top Level Department.

</p>
<br />

### 3. Configure Teams
<p>
<img src="https://github.com/user-attachments/assets/a678ad97-ce85-4ce1-a364-f748eaa109cb" height="80%" width="80%" alt="Configure Teams"/>
</p>
<p>
  
Navigate to Admin Panel → Agents → Teams.
 
Create a new team named Online Banking.
  
</p>
<br />

### 4. Allow Anyone to Create Tickets
<p>
<img src="https://github.com/user-attachments/assets/5f2bb4dc-15e8-46e4-8347-00e2465fd793" height="80%" width="80%" alt="Free Ticket Creation"/>
</p>
<p>
  
Navigate to Admin Panel → Settings → Users.

Uncheck "Require registration and login to create tickets".
  
</p>
<br />

### 5. Configure Agents (Workers)
<p>
<img src="https://github.com/user-attachments/assets/602d001b-c986-487d-a2a2-a2866ea859b7" height="80%" width="80%" alt="Configure Agents"/>
</p>
<p>
  
Navigate to Admin Panel → Agents → Add New.
  
Add two agents:
  
- Jane Doe: Assign to SysAdmins and Online Banking Team. Grant Supreme Admin permissions. Set the password to Password123.
  
- John Doe: Assign to Support Department with View-Only access. Set the password to Password123.
  
</p>
<br />

### 6. Configure Users (Customers)
<p>
<img src="https://github.com/user-attachments/assets/e9f7e243-a3c5-462a-8002-8e5ab429c9e1" height="80%" width="80%" alt="Configure Users"/>
</p>
<p>
  
Navigate to Agent Panel → Users → Add New.
  
Add a user named Karen with email karen@logoproductions.com.
  
</p>
<br />

### 6. Configure Service Level Agreements (SLA)
<p>
<img src="https://github.com/user-attachments/assets/17647f53-2203-43b8-9cd7-ca29df3a870d" height="80%" width="80%" alt="Configure Agents"/>
</p>
<p>
  
Navigate to Admin Panel → Manage → SLA.

Create three categories of SLA: Sev-A, Sev-B, Sev-C.

- Sev-A being a really bad problem with a grace period of 1 hour and 24/7 schedule.
  
- Sev-B being a normal problem with a grace period of 4 hours and 24/7 schedule.
  
- Sev-C being a moderate problem with a grace period of 8 hours and 25/7 schedule [business hours].

</p>
<br />

### 7. Configure Help Topics
<p>
<img src="https://github.com/user-attachments/assets/deb30f93-5c52-4e86-bed5-bc5241b9f197" height="80%" width="80%" alt="Configure Help Topics"/>
</p>
<p>
  
Navigate to Admin Panel → Manage → Help Topics.

Create help topics for user to select: Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, and Other.

</p>
<br />


