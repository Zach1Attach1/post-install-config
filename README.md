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

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Portal Setup: Establish separate URLs for the admin/analyst login and end-user access to clearly differentiate roles.
- Organizational Structure: Configure roles, departments, and teams to manage permissions and ticket visibility effectively.
- User Registration: Adjust settings to require registration for ticket submission, ensuring that only authenticated users can create tickets.
- Account Management: Create and assign accounts for both agents (with appropriate departmental affiliations) and end users.
- Service Configuration: Set up SLAs to define response times and configure help topics to streamline ticket categorization.

<h2>Configuration Steps</h2>

<h2>1. Organizational Setup:</h2>
In the Admin Panel, I established a clear structure by configuring roles, departments, and teams. I created a role such as “Supreme Admin” (via Agents → Roles) to manage high-level permissions, defined departments by assigning agents to “SysAdmins” for system-related issues and “Support” for customer queries, and set up teams like “Online Banking” (via Agents → Teams) to facilitate collaboration across different departments.

<h2>2. Ticket Submission Settings:</h2>
I controlled the ticket submission process by navigating to Admin Panel → Settings → User Settings and unchecking the option that allowed unregistered users to create tickets. This action ensured that users had to register and log in before submitting a support request, thereby tying every ticket to an authenticated user and streamlining follow-up communication.

<h2>3. Account and Service Configuration:</h2>
I configured both agent and end-user accounts and defined service parameters to optimize support operations. I added new agents (for example, Jane in the “SysAdmins” department and John in “Support”) via Admin Panel → Agents → Add New, and created user accounts for customers like Karen and Ken through Agent Panel → Users → Add New. Additionally, I set up service-level agreements (SLAs) under Admin Panel → Manage → SLA by establishing tiers such as Sev-A (1-hour grace period, 24/7 schedule), Sev-B (4-hour grace period, 24/7), and Sev-C (8-hour grace period during business hours), and configured help topics (e.g., Business Critical Outage, Password Reset) under Admin Panel → Manage → Help Topics to streamline ticket categorization and resolution.
<br />
