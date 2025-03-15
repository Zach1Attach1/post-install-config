# osTicket: Post-Installation Configuration

## Project Overview
This project demonstrates the post-installation configuration of osTicket, setting up the necessary roles, departments, teams, and other components to create a functioning help desk system.

## Environments and Technologies Used
- Microsoft Azure (Virtual Machine)
- Windows 10
- osTicket (Help Desk Ticketing System)
- Internet Information Services (IIS)

## Prerequisites
- osTicket successfully installed
- Admin access to osTicket

## Configuration Steps

### 1. Admin/Agent Panel Overview
- Accessed the Admin Panel using admin credentials
- Identified the differences between Agent and Admin panels
- Explored the interface layout and key features

![Admin Panel](https://i.imgur.com/T3V2cD0.png)

### 2. Configure Roles
Roles group permissions that can be assigned to Agents.

- Navigated to Admin Panel -> Agents -> Roles
- Created a new role: "Supreme Admin"
- Assigned all permissions to this role to allow full system access

![Roles Configuration](https://i.imgur.com/8wJpqjq.png)

### 3. Configure Departments
Departments determine ticket visibility and assignment.

- Navigated to Admin Panel -> Agents -> Departments
- Created "SysAdmins" department
- Configured as a top-level department to handle system-related issues
- Deleted the "Maintenance" department (not archived)

![Departments](https://i.imgur.com/zYDgrJ0.png)

### 4. Configure Teams
Teams allow pulling agents from different departments.

- Navigated to Admin Panel -> Agents -> Teams
- Created "Online Banking" team to handle financial system issues
- Team members can come from different departments but collaborate on banking issues

![Teams Configuration](https://i.imgur.com/YPARhNx.png)

### 5. Configure Agents (Workers)
Agents are the staff who work on tickets.

- Navigated to Admin Panel -> Agents -> Add New
- Created Agent "Jane" in SysAdmins department
- Created Agent "John" in Support department
- Assigned appropriate roles and team memberships

![Agents Configuration](https://i.imgur.com/1lqzJY8.png)

### 6. Configure User Registration Settings
- Navigated to Admin Panel -> Settings -> User Settings
- Required registration and login to create tickets for better tracking

### 7. Configure Users (Customers)
Users are the customers who submit tickets.

- Navigated to Agent Panel -> Users -> Add New
- Created users "Karen" and "Ken" as sample customers
- Set up their email addresses and basic information

![Users Configuration](https://i.imgur.com/KFdOmRo.png)

### 8. Configure SLA (Service Level Agreements)
SLAs define the timeframe for ticket resolution.

- Navigated to Admin Panel -> Manage -> SLA
- Created three tiers of service:
  - Sev-A: 1 hour response time, 24/7 schedule (critical issues)
  - Sev-B: 4 hour response time, 24/7 schedule (high priority)
  - Sev-C: 8 hour response time, business hours (normal priority)

![SLA Configuration](https://i.imgur.com/AZlXJEv.png)

### 9. Configure Help Topics
Help Topics categorize tickets for proper routing.

- Navigated to Admin Panel -> Manage -> Help Topics
- Created the following topics:
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other

![Help Topics](https://i.imgur.com/uc4MQdW.png)

## Lessons Learned
- Understanding role-based access control in help desk systems
- The importance of proper SLA configuration for prioritizing work
- How departments, teams and agents work together in a ticket workflow
- Methods of categorizing and routing support requests efficiently
- The difference between user (customer) and agent experiences
