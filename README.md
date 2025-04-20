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
👥 Configuring User Roles in osTicket
Now that we have osTicket installed and running, it’s time to configure and assign roles to the users we created earlier.

🧑‍💼 Understanding Roles in osTicket
Roles in osTicket are customizable access profiles that define what each user or agent can do within the system.
As the administrator, you have full control over assigning permissions based on your organization’s needs.

⚙️ Creating a Custom Role
Log in to the osTicket Admin Panel.
Navigate to the Agent Panel.
Click on Agents → Roles.

➕ Add a New Role
Click “Add New Role.”
For this example, name the role:
Supreme Admin

Assign Full Permissions to this role. This gives the user complete access to perform tasks such as:
Assigning tickets
Responding to tickets
Managing ticket workflows
Viewing and editing user information
Save the role.

</p>
<br />

Step 2
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 18 42 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/f599a5d9-6d75-4caa-abc9-960f7a748a2a">
</p>
<p>
🏢 Configuring Departments in osTicket
Next, we’ll configure departments in osTicket — an important step for organizing your support structure.

🧩 What Are Departments?
Departments are groups of agents that handle specific types of tickets.
Examples include:

Support
Maintenance
Finance
Each department has visibility and responsibility over tickets related to their domain.
Departments can also collaborate or reassign tickets to one another when needed.

🛠️ Creating a Department
Log in to the Agent Panel.
Navigate to Agents → Departments.
Click “Add New Department.”
For this example, name the department:
System Administrators
Leave the settings at their default values.
Click “Create Department” to save it.

</p>
<br />

Step 3
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 29 52 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/a8a1c0bd-d527-4b07-a276-e3e4e11fd7c5">
</p>
<p>
👨‍👩‍👧‍👦 Configuring Teams in osTicket
Now we’ll set up Teams, which allow you to group agents from different departments to work together on specific issues or help topics.

🧠 Why Use Teams?
Teams are flexible groups that aren’t limited to a single department.
They’re useful for:

Tackling high-priority tickets
Handling escalations
Collaborating across specialties
This helps streamline workflows and improve resolution times.

🛠️ Creating a Team

Log in to the osTicket Agent Panel.
Navigate to Agents → Teams.
Click “Add New Team.”

✏️ Example Setup

For demonstration purposes, let’s create two teams:

Support Level 1
Support Level 2
These teams can handle different tiers of support based on complexity or urgency.

Name each team accordingly and configure any optional settings based on your needs.
Click “Create Team” to save.

</p>
<br />

Step 4
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 37 16 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/97ecb899-13ae-41ec-b684-68e74006a91c">
</p>
<p>
📝 Allowing Anyone to Create Tickets in osTicket
Now, we’ll adjust the settings so that anyone can create and submit tickets, regardless of whether they have an account or not.

🔑 What Does This Setting Do?

By default, osTicket may require users to register before they can submit tickets.
Unchecking this setting will allow anyone, including unregistered users, to create tickets without an account.

🛠️ Modifying User Settings

Log in to the Admin Panel.
Navigate to Settings → User Settings.
Look for the setting labeled “Registration Required.”
Uncheck the box next to “Registration Required.”

</p>
<br />

Step 5
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 10 56 21 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/3b709453-218b-4e3d-9412-d9047dd6e0c5">
</p>
<p>
🧑‍💻 Configuring New Agents
Now it’s time to configure agents, who are the help desk professionals responsible for managing and resolving submitted tickets.

🧑‍💼 What Are Agents?

Agents are users with special permissions who can:

View and manage tickets
Communicate with customers
Resolve issues and close tickets
🛠️ Adding New Agents

Log in to the Agent Panel.
Navigate to Agents → Add New.
Fill in the details for each agent. For our example, we’ll add:
Jane
John
Assign the appropriate roles and permissions based on their responsibilities.
Click Save to add them as agents.

</p>
<br />

Step 6
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 07 54 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/c730b4c8-42ff-4be2-b3bc-b68ea88b251f">
</p>
<p>
👥 Configuring Users in osTicket
Next, we’ll set up the users in osTicket. These users represent customers or clients who are submitting tickets for support, whether it’s for issues with their computers, software updates, or other technical concerns.

🧑‍💻 What Are Users?

Users are the individuals who will:

Submit tickets for technical assistance
Provide details about their issues
Interact with agents who will resolve their concerns
In this step, we’re simulating the process of an IT help desk professional working on tickets for clients.

🛠️ Adding New Users

Log in to the Agent Panel.
Navigate to Users → Add New.
Add two new users for this example:
Karen
Ken
Fill in the necessary user details and click Save to add them.

</p>
<br />

Step 7
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 21 59 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/aec89ec1-0d7a-403f-932c-996d0f94b7df">
</p>
<p>
🕒 Configuring SLA Plans in osTicket
Now, we’ll configure SLA (Service Level Agreement) Plans. These plans define the timeframes within which tickets must be addressed or resolved by agents.

⚖️ What Are SLA Plans?

SLA Plans set the priority and deadlines for tickets based on their severity or urgency. These plans help:

Prioritize issues (e.g., critical vs. low priority)
Establish clear timeframes for resolving tickets
Ensure that agents respond promptly within designated time limits
🛠️ Creating SLA Plans

Log in to the Agent Panel.
Navigate to Manage → SLA.
Create three different SLA plans with varying levels of urgency:
SEV-A (Critical Issues)
Resolution Time: 1 hour
Active Time: 24/7
SEV-B (High Priority Issues)
Resolution Time: 4 hours
Active Time: 24/7
SEV-C (Low Priority/Common Issues)
Resolution Time: 8 hours
Active Time: Business Hours
Save each SLA Plan after configuration.

</p>
<br />


Step 8
<p>
<img width="1385" alt="Screenshot 2023-09-26 at 11 29 55 PM" src="https://github.com/lucasfregoso/post-install-config/assets/144977615/25b5f328-bc05-44c2-ab48-6fb516ca9597">
</p>
<p>
📝 Configuring Help Topics in osTicket
Finally, we’ll configure Help Topics. These topics are presented to end users (like Ken and Karen) when they submit a ticket. They can select the topic that best matches their issue, streamlining the process for both users and agents.

🎯 What Are Help Topics?

Help Topics provide predefined categories for end users to choose from when submitting tickets. This helps to:

Guide users in selecting the most relevant issue category
Ensure tickets are routed correctly for faster resolution
Make ticket submission more efficient for both users and support agents
🛠️ Creating Help Topics

Log in to the Admin Panel.
Navigate to Manage → Help Topics.
Add the following help topics that end users can choose from:
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Save each help topic after adding them.

</p>
<br />
















