<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post Installation Configuration</h1>
This tutorial outlines the post installation configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (22H2)

<h2>List of Prerequisites</h2>

- Step 1
- Step 2
- Step 3
- Step 4
- Step 5
- Step 6
- Step 7
- Step 8

(Images going from left to right)
<h2>Installation Steps</h2>

Step 1
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 00 02 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/a15ef5c9-c5c7-49df-a695-92825ec9a3d8">
</p>
<p>
For our first step, we are going to configure and assign roles to the users we created in the previous part and the roles are essentially custom because we will define the roles for who will have access to do what and how much. So as the admin, in osTicket we go to 'Agent Panel', 'Agents', and then 'Roles' Once we are here, we add a new role and name it 'Supreme Admin' for our example, then we allow the 'Supreme Admin' to have all permissions, which basically allows this user to do things such as assign tickets, do tickets themselves, reply to messages, etc. 
</p>
<br />

Step 2
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 18 42 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/f599a5d9-6d75-4caa-abc9-960f7a748a2a">
</p>
<p>
Our second step is going to be configuring departments and these are basically a collection of agents for said department. Support, maintenaince, finance are some examples of this and department members will see tickets assigned to their area of expertise and sometimes departments will reach out to other departments for a collaboration or to reassign a ticket. But, for this part all we have to do is go to 'Agent Panel', 'Agents', then 'Departments' and add our 'System Administrators' department with the default settings. 
</p>
<br />

Step 3
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 29 52 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/a8a1c0bd-d527-4b07-a276-e3e4e11fd7c5">
</p>
<p>
Next, we are going to configure our teams and teams allows agents to be pulled from differing departments organizing them to tackle a specific issue, help topic, or a ticket. With that said, in osTicket we go to 'Agent Panel', 'Agents', and 'Teams.' From here we just add new team and this could be whatever you want depending on what is needed in a company/business, but for our example we added support level 1 and support level 2. 
</p>
<br />

Step 4
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 37 16 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/97ecb899-13ae-41ec-b684-68e74006a91c">
</p>
<p>
Next, we are going to allow anyone to create tickets by going to 'Admin Panel', 'Settings', 'User Settings', and under 'Registration Required' we want to make sure that is unchecked allowing anyone to be able to create and submit tickets. 
</p>
<br />

Step 5
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 56 21 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/3b709453-218b-4e3d-9412-d9047dd6e0c5">
</p>
<p>
Next, we are going to configure new agents and our agents are essentially our help desk professionals that look through the tickets submitted as well as solving them. So, we go to 'Agent Panel', 'Agents', 'Add New', and create our workers Jane and John.
</p>
<br />

Step 6
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 07 54 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/c730b4c8-42ff-4be2-b3bc-b68ea88b251f">
</p>
<p>
Next, we are going to configure the users and the users in this lab are our customers or clients who are having specific issues with their computers, their company's online banking system, software update, and so on. These are the people who we will be providing our support to. We are basically simulating an IT help desk professional working on tickets. To add them, we go to 'Agent Panel', 'Users', 'Add New' and add Karen and Ken as our users.
</p>
<br />

Step 7
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 21 59 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/aec89ec1-0d7a-403f-932c-996d0f94b7df">
</p>
<p>
Next, we will configure our SLA Plans and these in osTicket determine the length of time in which the help desk professional has until a ticket(s) needs to be completed. So we created three different SLA Plans with 'SEV A' being our high priority or critical issue and 'SEV C' being our low priority or our common issue that people may have. Of course, with these plans having different levels they will also have different deadlines and for which ever one it doesn't matter what day of the week it is, if it falls within an acitve timeframe then the issue needs to be resolved. So, in the lab we again migrate to 'Agent Panel', 'Manage', 'SLA' and add our 'Sev-A(1 hour 24/7)', 'Sev-B(4 hours 24/7)', 'Sev-C(8 hours, buiness hours).'
</p>
<br />


Step 8
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 29 55 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/25b5f328-bc05-44c2-ab48-6fb516ca9597">
</p>
<p>
Lastly, we are going to configure help topics and this is for our end users, so in our lab it would be Ken and Karen who will be able to choose from our list of topics that we created, which will allow them to determine which topic best fits their issue. So we go to 'Admin Panel', 'Manage', 'Help Topics' and we add the following help topics: Business Critical Outage, Personal Computer Issues, Equipment Request, and Password Reset. 
</p>
<br />
















