<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Explore osTicket
- Login to osTicket
- 

<h2>Configuration Steps</h2>

</p>
<br />

![image](https://github.com/user-attachments/assets/1898f29d-3184-43e1-9608-3b2895de5240)

</p>
<br />

First in the browser type in "http://localhost/osTicket/scp/login.php", this will take you to the osTicket Admin/Agent login page.

Next create a new tab and type in "http://localhost/osTicket/", this will taek you to the osTicket End User page to create tickets.

</p>
<br />

![image](https://github.com/user-attachments/assets/f1c5cd87-963b-4291-a4fe-a16227541185)

</p>
<br />

Go to the Admin/Agent login page, input the credentials you used when setting up osTicket and login.

When logged in as the admin, the first panel you see is the agent panel, this lets you see tickets and gives you a view of what the agents will see when responding to tickets. in the upper right corner of the screen you will see "Admin Panel", click on it.

</p>
<br />

![image](https://github.com/user-attachments/assets/562e5d19-3de8-4dd7-9b6a-7fb053d51d1b)

</p>
<br />

This is the Admin panel it is used for configuration, creating agents, teams, and departments, and to edit them as well.

Next were going to configure Roles, in the Admin panel, click the big agents heading, then click roles

</p>
<br />

![image](https://github.com/user-attachments/assets/3e4bded3-f3bc-4362-b0f5-190ca715485b)

</p>
<br />

Roles are different levels of access permissions that you can assign to agents.

Click add new role, next you can type a name like "Supreme Admin", clck permissions, and you can set what permissions you want. For Supreme Admin we can check all the boxes. Then click add role to create the new role. 

![image](https://github.com/user-attachments/assets/5dd38299-f612-423a-8f1c-1090b648f9a1)

![image](https://github.com/user-attachments/assets/c35482b8-bdad-4f3b-a70b-6bd2e092fe9a)

Next we can configure Departments, Depatments are used for Ticket visibility, this lets tickets get assigned to certain departments so that the agents within the department can see their tickets. It can also be configured to where departments can only see tickets assigned to their respective department. 

Click on departments, this is a list of all the departments. 

![image](https://github.com/user-attachments/assets/8d0cf399-335c-4796-8580-2bc40267a21a)

Lets create a new department for Sys Admins, and delete the Maintenance department we do not need. Click Add new department, 


























