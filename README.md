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

- Windows 10 Pro </b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Login to the osTicket Admin Panel
- Configure Roles
- Configure Departments
- Configure Teams
- Configure Help Topics

<h2>Configuration Steps</h2>
<p> Login to the osTicket Admin Panel. Below displays the tickets for admin/helpdesk User Interface (UI) that will reflect the tickets that are created by the End User http://localhost/osTicket/scp/login.php

</p>
<p align="center">

![256C875F-F717-4BB2-9524-2A46BFDEE205_1_105_c](https://github.com/stevelloyd76/post-install-config/assets/162848869/259737ad-fa4e-4296-a732-b8dd6863d498)

</p>

<br />
<details>
 <summary><b>- Configure</b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">[Roles]</a></summary>
 <br /> 
Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access. An unlimited number of roles can be created and assigned to Agents with access to various departments.
    <ol>
  <li>Admin Panel -> Agents -> Roles</li>
  <li>Supreme Admin</li>
    </ol>
<p align="center">

<br />
<p> Now we can enable the <a href="https://docs.osticket.com/en/latest/Features/Visibility%20Permissions.html">permissions</a> for this role and as the "Supreme Admin" we've enabled every possible permission available.  
<p align="center">

</p>
</details>    
<hr>
<p>
 <details>   
 <summary><b>- Configure</b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">[Departments]</a></summary>
     <br />
  Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department.
    <ol>
    <li>Admin Panel -> Agents -> Departments</li>
    <li> System Administrators</li>
    <li>Leave the remaining fields set as default and simply review what selections are available to choose from</li> 
      </ol>
</p>
  </p>
</details>   
  <hr>
<details>
  <summary><b><i>- Configure </i></b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">[Teams]</a></summary>
    <br />
  Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter.
  <ol><li>Admin Panel -> Agents -> Teams</li>
    <li>Level I Support </li>
    <li>Level II Support </li>
</ol>
<p align="center">
   
 </p>
-<b>Allow anyone to create tickets </b> in <a href="https://docs.osticket.com/en/latest/Admin/Settings/Users.html?highlight=registration">User Settings</a> <br />
Registration can be required for Users to create tickets on the Help Desk to prevent random tickets or to limit Users’ accessibility to the help desk.
   <ol>
    <li>Admin Panel -> Settings -> User Settings </li>
    <li>Registration Required: Require registration and login to create tickets -for this lab, we will leave it unchecked so that tickets can be created without restrictions/limitations</li>
    </ol>
    
</details>      
  <hr>
<details>
  <summary> <b><i>- Configure</b></i> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">[Agents (workers)]</a></summary>
      <br />
Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent’s Profile.
    <ol>Admin Panel -> Agents -> Add New
    <li>Jane</li>
        <li>John </li>
        </ol>
 
  </details>
    <hr>
  <details>    
- <summary><b><i>- Configure</i></b> <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">[Users (customers)]</a></summary> 
      <br />
Users (customers) can create an account and log in to create a ticket or check on their ticket status as well.
<ol>Agent Panel -> Users -> Add New
        <li>Karen</li>
        <li>Ken</li>
</ol>
<p align="center">
    
</p>
 </details>    
    <hr>
<details>      
    <summary> <b><i>- Configure</b></i> <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">[SLA]</a></summary>
        <br />    
SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.
    Admin Panel -> Manage -> SLA
    <ol>
    <li>Sev-A (1 hour, 24/7)</li>
    <li>Sev-B (4 hours, 24/7)</li>
    <li>Sev-C (8 hours, business hours)</li>
    </ol>
    
<p align="center">
    
  ![2D45CE17-15A5-4DBD-BED2-CD0F07446C00_1_105_c](https://github.com/stevelloyd76/post-install-config/assets/162848869/cc26241e-e11d-4611-889d-14b9ab7954a8)
  
</p>
</details>        
<hr>
<details>        
<summary><b><i>- Configure </b></i> <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html?highlight=help%20topics">Help Topics</a></summary> <br />
Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for further breakdown (For example, Human Resources and Human Resources/Payroll.)
     <h5>Admin Panel -> Manage -> Help Topics</h5>
        <li> Business Critical Outage </li>
        <li> Personal Computer Issues </li>
        <li> Equipment Request </li>
        <li> Password Reset </li>
 
<br />
<p align="right"> Next up, <a href="https://github.com/0xbythesecond/ticket-lifecycle"
>Ticket Lifecycle </a></p>
</details>
