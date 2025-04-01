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

- Windows 10</b> (Standard DS2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Add Teams
- Assign Agents
- Configure Users
- Set SLA's

<h2>Configuration Steps</h2>

<p>
</p>
<p>
🔐 Login Pages

- **Admin/Analyst Login Page**  
  [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)

- **End User Portal**  
  [http://localhost/osTicket](http://localhost/osTicket)

---
</p>
<br />


<p>
</p>
<p>
👤 Agent Panel vs Admin Panel

- **Agent Panel**: For support agents to manage tickets.
- **Admin Panel**: For administrators to configure the system (users, roles, SLAs, etc.).

---
</p>
<br />


<p>
<img src="https://i.imgur.com/68I3FP5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
🛡️ Configure Roles

> Used to group and define agent permissions.

**Navigation**: `Admin Panel -> Agents -> Roles`

- Create a new role: `Supreme Admin`

---
</p>
<br />


<p>
<img src="https://i.imgur.com/gYpeckB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 🏢 Configure Departments

> Determines ticket visibility and responsibility split.

**Navigation**: `Admin Panel -> Agents -> Departments`

- Add department: `SysAdmins`

Examples:
- Help Desk
- SysAdmins
- Networking

---
</p>
<br />



<p>
<img src="https://i.imgur.com/QGtgvEy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
👥 Configure Teams

> Teams allow agents from different departments to work together.

**Navigation**: `Admin Panel -> Agents -> Teams`

- Create team: `Online Banking`

---
</p>
<br />





<p>
<img src="https://i.imgur.com/auQkCbp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 🎫 Ticket Creation Settings

**Navigation**: `Admin Panel -> Settings -> User Settings`

- ✅ Allow anyone to create tickets:
  - **UNCHECK**: "Require registration and login to create tickets"

---
</p>
<br />


<p>
<img src="https://i.imgur.com/b58vLNo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
👨‍💼 Configure Agents (Internal Workers)

**Navigation**: `Admin Panel -> Agents -> Add New`

- Add agent: `Jane`  
  - Department: `SysAdmins`

- Add agent: `John`  
  - Department: `Support`

---

</p>
<br />


<p>
<img src="https://i.imgur.com/0UYWjww.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
👨‍👩‍👧 Configure Users (External Customers)

**Navigation**: `Agent Panel -> Users -> Add New`

- Add user: `Karen`
- Add user: `Ken`

---
</p>
<br />


<p>
<img src="https://i.imgur.com/efquR2u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
⏱️ Configure SLA (Service Level Agreements)

**Navigation**: `Admin Panel -> Manage -> SLA`

Create SLAs:

- `Sev-A`  
  - Grace Period: 1 hour  
  - Schedule: 24/7

- `Sev-B`  
  - Grace Period: 4 hours  
  - Schedule: 24/7

- `Sev-C`  
  - Grace Period: 8 hours  
  - Schedule: Business Hours

---

</p>
<br />


<p>
<img src="https://i.imgur.com/kVFcWoT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
📝 Configure Help Topics

> These are the categories users pick from when submitting tickets.

**Navigation**: `Admin Panel -> Manage -> Help Topics`

Add Help Topics:

- Business Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  
- Other
</p>
<br />


