<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>High Level List of Steps</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Download and install the Rewrite Module
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLAs
- Configure Help Topics

<h2>Configuration Visual Walkthrough</h2>

<p>
<img src="https://i.imgur.com/fYi42rM.png"/>
</p>
<p>
First log into osTicket with the credentials that we set for the admin user in the previous tutorial.
</p>
<br />

<p>
<img src="https://i.imgur.com/smoRDS8.png"/>
</p>
<p>
Then go to the admin panel, that button will switch from "Admin Panel" to "Agent Panel" when you get to the admin panel.
</p>
<br />

<p>
<img src="https://i.imgur.com/B6eLqcE.png"/>
</p>
<p>
Then go to Agents -> Roles -> Add New Role
</p>
<br />

<p>
<img src="https://i.imgur.com/dKzlDpy.png"/>
</p>
<p>
Now name the new role "Supreme Admin" and select all permissions for Tickets, Tasks, and Knowledgebase, then click save.
</p>
<br />

<p>
<img src="https://i.imgur.com/fujykeu.png"/>
</p>
<p>
then go to the departments panel and add a new department.
</p>
<br />

<p>
<img src="https://i.imgur.com/awbVYtb.png"/>
</p>
<p>
Name it "SysAdmins" and hit create.
</p>
<br />

<p>
<img src="https://i.imgur.com/px2oFmM.png"/>
</p>
<p>
Now go to the Teams panel and hit add new team, then name it "Level II Support" and create team.
</p>
<br />

<p>
<img src="https://i.imgur.com/55PgdlN.png"/>
</p>
<p>
Now go to Settings -> Users -> * Settings and make sure the authentication settings make the screenshot above.
</p>
<br />

<p>
<img src="https://i.imgur.com/zgW8RYK.png"/>
</p>
<p>
Now go into the agents panel and add new agent.
</p>
<br />

<p>
<img src="https://i.imgur.com/VbdAyYo.png"/>
<img src="https://i.imgur.com/bOpYXec.png"/>
</p>
<p>
Now add the following accounts:

- Name:	Jane Doe
- Email Address: jane.doe@osticket.com
- Username: jane.doe
- Set the password to "Password1" (you might need to uncheck that send agent password reset email box)
- Go to Access and set the department to SysAdmins and select Supreme Admin for the role.
- Go to the teams section and select Level II Support, then create.
  
Then repeat those same exact steps for John Doe.
</p>
<br />

<p>
<img src="https://i.imgur.com/OOQdVmW.png"/>
</p>
<p>
Then go to Agent panel -> Users -> Add User
</p>
<br />

<p>
<img src="https://i.imgur.com/6uBqz01.png"/>
</p>
<p>
Then add the following users:
 
- Email Address: karen@osticket.com
- Full Name: Karen
  
- Email Address: ken@osticket.com
- Full Name: Ken
</p>
<br />

<p>
<img src="https://i.imgur.com/mdD3pzb.png"/>
</p>
<p>
Then go to Admin Panel -> Manage -> SLA -> Add New SLA Plan
</p>
<br />

<p>
<img src="https://i.imgur.com/AFDwYsq.png"/>
</p>
<p>
Now add the following SLAs
  
- SEV-A with a grace period of 1 hour, and a 24/7 schedule
- SEV-B with a grace period of 4 hours, and a 24/7 schedule
- SEV-C with a grace period of 8 hours, and a Mon-Fri business hours schedule
</p>
<br />

<p>
<img src="https://i.imgur.com/YL0FxCx.png"/>
</p>
<p>
Now go to "Help Topics" and add the following help topics:
  
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
  
The next tutorial we will explore tickets and the ticket lifecycle (link to that is listed below)
  
- [osTicket: Ticket Lifecycle Examples](https://github.com/aniyahelder/ticket-lifecycle.git)
</p>
<br />
