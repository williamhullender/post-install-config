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

- Login to osTicket
- Explore osTicket
- Configure and Add:
    - Roles
    - Departments
    - Teams
    - Agents (workers)
    - Users (customers)
    - SLAs
    - Help Topics
 - Allow anyone to create tickets

<h2>Related Projects</h2>

- [osTicket: Prerequisites and Installation](https://github.com/williamhullender/osticket-prereqs)
- [osTicket: Ticket Lifecycle Examples](https://github.com/williamhullender/ticket-lifecycle)

<h2>Configuration Steps</h2>

</p>
<br />

![image](https://github.com/user-attachments/assets/1898f29d-3184-43e1-9608-3b2895de5240)

</p>
<br />

First in the browser type in "http://localhost/osTicket/scp/login.php", this will take you to the osTicket Admin/Agent login page.

Next create a new tab and type in "http://localhost/osTicket/", this will take you to the osTicket End User page to create tickets.

</p>
<br />

![image](https://github.com/user-attachments/assets/f1c5cd87-963b-4291-a4fe-a16227541185)

</p>
<br />

Go to the Admin/Agent login page, input the credentials you used when setting up osTicket and login.

When logged in as the admin, the first panel you see is the agent panel, this lets you see tickets and gives you a view of what the agents will see when responding to tickets. in the upper right corner of the screen you will see "Admin Panel", click on it.

</p>
<br />

![image](https://github.com/user-attachments/assets/e45d243d-128d-46bf-916b-c0db19c02f5b)

</p>
<br />

This is the Admin panel, it is used for configuration, creating agents, teams, and departments, and to edit them as well.

Next were going to configure Roles, in the Admin panel, click the big agents heading, then click the roles tab.

</p>
<br />

![image](https://github.com/user-attachments/assets/3e4bded3-f3bc-4362-b0f5-190ca715485b)

</p>
<br />

Roles are different levels of access permissions that you can assign to agents.

Click add new role, next you can type a name like "Supreme Admin", next click permissions. Here you can set what permissions you want. For Supreme Admin we can check all the boxes. Then click add role to create the new role. 

</p>
<br />

![image](https://github.com/user-attachments/assets/5dd38299-f612-423a-8f1c-1090b648f9a1)

</p>
<br />

![image](https://github.com/user-attachments/assets/c35482b8-bdad-4f3b-a70b-6bd2e092fe9a)

</p>
<br />

Next we can configure Departments, Depatments are used for Ticket visibility, this lets tickets get assigned to certain departments so that the agents within the department can see their tickets. It can also be configured to where departments can only see tickets assigned to their respective department. 

Click on departments, this is a list of all the departments. 

</p>
<br />

![image](https://github.com/user-attachments/assets/8d0cf399-335c-4796-8580-2bc40267a21a)

</p>
<br />

Lets create a new department for Sys Admins, and delete the Maintenance department we do not need. 

Click Add new department, leave it as a Top Level Department, type name in as "SysAdmins".

</p>
<br />

![image](https://github.com/user-attachments/assets/306f8141-8ead-44f9-83fd-06913672f925)

</p>
<br />

In the Access tab, that allows you to add Agents to the department, at this time we have no Agents in the system to add. 

Now click Create Dept at the bottom to create the new department.

</p>
<br />

![image](https://github.com/user-attachments/assets/82bfe7fb-c40f-47db-b7b4-8aaadfdcd4e5)

</p>
<br />

Now we can delete the Maintenance department as we do not need it.

Click the Departments tab to see all the departments under the Agents heading. Click the box next to the Maintenance department, and on the right side click the drop down arrow next to More. Click delete -> then click Yes, Do it!

</p>
<br />

![image](https://github.com/user-attachments/assets/c65778c6-f13a-40a3-831a-f9246216e1e5)

</p>
<br />

Next we can configure teams, Teams lets you pull Agents from different departments and lets  you assign tickets to a specific team. Lets create a team for online banking.

In the Agents heading, click Teams. Then click Add New Team. Then type in the name "Online Banking". 

If you click the Members tab, this lets you add members onto the team. 

Next click Create Team to create the team.

</p>
<br />

![image](https://github.com/user-attachments/assets/8c5f017f-2d78-4d1b-9a33-5df9a5c64d14)

</p>
<br />

Next we are going to configure osTicket to allow anyone to create tickets, even if they are not registered.

Ensure you are in the Admin panel (you are in admin panel when in the top right of screen it says Agent Panel)

</p>
<br />

![image](https://github.com/user-attachments/assets/be54ab6f-94d8-43f5-8019-b4f79163fb5f)

</p>
<br />

Click the Settings heading, then click Users. Make sure the box beside Require registration and login to create tickets is unchecked. Then click Save Changes.

</p>
<br />

![image](https://github.com/user-attachments/assets/62da5c79-aaef-4274-b24d-6177366fd955)

</p>
<br />

Next we can configure Agents, Agents are the employees that can reply, assign, change, work on, or resovle tickets.

Click on the Agents header, then click on agents.

</p>
<br />

![image](https://github.com/user-attachments/assets/406ca3f8-e8ea-4271-942a-70aa277861de)

</p>
<br />

We can add two new agents, one agent for each department we have.

Click on Add New Agent, then we can fill out the information for the new Agent, we can use the name "Jane
Doe" and give her a random email and phone number, then we can give her a username (ensure you remember the username and password info, as we will need this to login in the next project). I used username: "JaneD", then click Set Password

</p>
<br />

![image](https://github.com/user-attachments/assets/f1819ddf-1cc7-43cd-ae2e-9a43c1beba3f)

</p>
<br />

After clicking Set Password, ensure the box Send the agent a password reset email is unchecked so you can set the password.

Type in a password for JaneD and ensure to remember it or write it down. Then ensure the box Require password change at login is unchecked. Once done click Set.

</p>
<br />

![image](https://github.com/user-attachments/assets/66e7ef6e-57bd-4b32-8db7-7a48ed2b9eed)

</p>
<br />

Next click the Access tab, this is where you can assign a new agent to a department and set roles.

Click the Select Department drop down under Primarty Department and select SysAdmins, then select Role as Supreme Admin.

</p>
<br />

![image](https://github.com/user-attachments/assets/7d991f44-95cd-4615-a315-2dd8f83f5a20)

</p>
<br />

The permissoions tab lets you customize the Agents permissions.

Next click the Teams header, and click the Select Team dropdown and select Online Banking and click Add to add Jane to the Online Banking team. Once done, click Create.

</p>
<br />

![image](https://github.com/user-attachments/assets/9159fbf9-a1b2-4f21-b55c-bd06db659902)

</p>
<br />

Next were gonna repeat the same process for "John Doe" but we will add him to a different department and give him a different Role.

Click Add New Agent again. And repeat the same steps for Jane but for John and ensure to remember or write down the username and password for the next project.

</p>
<br />

![image](https://github.com/user-attachments/assets/e7f13daf-ef64-426f-a352-436602df97f4)

</p>
<br />

Next click the Access tab, then put John in the Support department, with the Role of All Access. We can leave everything else as is and click Create.

</p>
<br />

![image](https://github.com/user-attachments/assets/c22bc111-8a37-45f9-bb6a-151e9d9db7d6)

</p>
<br />

Now when you click the agents tab, underneath the Agents header, you should see 3 Agents now. Jane, John, and your default admin account.

</p>
<br />

![image](https://github.com/user-attachments/assets/004cbede-f749-4d71-805f-d051e669c8d9)

</p>
<br />

Next we can configure Users to add customers into the ticketing system. We can add 1 user named Karen.

In the Agent Panel (click Agent Panel in top right of screen, should see "Admin Panel" when in Agent Panel), click the Users header, then click the User Directory tab. Then click Add User.

</p>
<br />

![image](https://github.com/user-attachments/assets/95e772ff-4ba2-4fd4-9295-4d5e9edcda2c)

</p>
<br />

Now we can fill out the Users name and email address. Then click Add User.

</p>
<br />

![image](https://github.com/user-attachments/assets/2709957b-34d5-4dab-820a-24dd9ce35b87)

</p>
<br />

Now when you click the User Directory tab, you will see your new user Karen.

</p>
<br />

![image](https://github.com/user-attachments/assets/aecbca6e-06ae-47f5-a4c4-4b1430a34085)

</p>
<br />

Next we can configure SLAs or Service Level Agreements.

To configure SLAs, in the Admin Panel, click the Manage header, then click the SLA tab. 

</p>
<br />

![image](https://github.com/user-attachments/assets/ff247b85-e022-4b0f-8047-11932f5d624a)

</p>
<br />

For this project and the next projects purpose, we will have 3 different SLA severity levels. 

- Sev-A (Grace Period: 1 hour, Schedule: 24/7)
- Sev-B (Grace Period: 4 hours, Schedule: 24/7)
- Sev-C (Grace Period: 8 hours, Schedule: Business Hours)

The grace period is how long Agents have to respond to a ticket before it becomes overdue, while the Schedule decides how the hours for the grace period react with weekends and after business hours, Sev-A counts down 24/7, while for Sev-C the grace period timer only counts down during business hours.

To create these SLAs, click Add New SLA Plan, then type in the name "Sev-A". Input the grace period of 1 hour, and give it the Schedule 24/7. Then click Add Plan.

</p>
<br />

![image](https://github.com/user-attachments/assets/e36b4b07-4eeb-463c-aa2f-f3ae1cb5bab5)

</p>
<br />

Now repeat these steps for the next two SLA levels using the information above for Sev-B and Sev-C.

</p>
<br />

![image](https://github.com/user-attachments/assets/068add9e-7e6b-42ae-bd1b-85ff0749971b)

</p>
<br />

![image](https://github.com/user-attachments/assets/8518e770-e372-463d-9291-d796a12fdf78)

</p>
<br />

Now we should have all three SLAs added in.

</p>
<br />

![image](https://github.com/user-attachments/assets/967f5961-fb45-479d-a70a-88fc8171bf7c)

</p>
<br />

Next we can configure Help Topics for Users/customers to categorize their ticket based on the type of problem they have.

In Admin Panel, click the Manage header, then click the Help Topics tab.

</p>
<br />

![image](https://github.com/user-attachments/assets/7ad17dc5-94fc-4da3-8486-29df700746b6)

</p>
<br />

For the purpose of this project and the next project we will add the following Help Topics:

- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

To add Help Topic, click Add New Help Topic.

Now enter in the Topic's name, then for the Parent Topic drop down select Report a Problem. Then click Add Topic.

</p>
<br />

![image](https://github.com/user-attachments/assets/6fbfbe90-ecad-44cc-8f33-0a2c8b64b066)

</p>
<br />

Then go back to the Help Topics tab, and repeat these steps for the rest of the Help Topics.

When you get to Equipment Request and Other, their Parent Topic is General Inquiry.

</p>
<br />

![image](https://github.com/user-attachments/assets/cfb6f0d0-b225-4ff2-aa85-69664df57b68)

</p>
<br />

![image](https://github.com/user-attachments/assets/bb8c3a29-03fe-45ba-a35f-d92bcf70cc0b)

</p>
<br />

![image](https://github.com/user-attachments/assets/825132ae-f5dd-4eea-9629-19f49dfbb4df)

</p>
<br />

![image](https://github.com/user-attachments/assets/f899d726-3a76-4d1d-8df9-153021168f71)

</p>
<br />

After you have completed all of these, your Help Topics list should look like this.

</p>
<br />

![image](https://github.com/user-attachments/assets/88a6ab79-960d-4d98-b877-9ac1b1aa33c2)

</p>
<br />

Once this is all done, Congratulations!, you have successfully configured your osTicket help desk ticketing system and are ready to create and resolve tickets.
