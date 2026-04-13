<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project focuses on the post-installation configuration of the osTicket help desk system. After starting osTicket, administrations settings were changed, including roles, departments, teams, agents, users, SLAs, and help topics. The goal was to simulate a real-world IT support environment by organizing ticket workflows, defining access control, and establishing service-level expectations.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- osTicket installed
- Access to Admin panel and Agent panel
- Understanding of help desk workflows, user and role management, and SLAs

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The system was accessed through a web browser using the Admin/Analyst login page (http://localhost/osTicket/scp/login.php) and the End User portal (http://localhost/osTicket/). The differences between the Agent Panel and Admin Panel were reviewed to understand their respective functionalities.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Roles were created in the Admin Panel under Agents → Roles to define permission levels. A “Supreme Admin” role was established to grant full system access and control over configurations.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Departments were set up in the Admin Panel under Agents → Departments to control ticket visibility and organization. A “SysAdmins” department was created to handle system-related support requests.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Teams were configured under Agents → Teams to allow collaboration across departments. An “Online Banking” team was created to group agents from different departments working on similar tasks or services.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
User access settings were modified in the Admin Panel under Settings → User Settings. The option allowing unregistered users to create tickets was disabled, requiring users to register and log in before submitting support requests.
</p>
<br />
  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agents (support staff) were added through the Admin Panel under Agents → Add New. Two agents were created: Jane, assigned to the SysAdmins department, and John, assigned to the Support department.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
End users (customers) were added through the Agent Panel under Users → Add New. Two users, Karen and Ken, were created to simulate customer interactions within the help desk system.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Service Level Agreements (SLAs) were configured under Manage → SLA in the Admin Panel. Three SLA levels were created: Sev-A with a 1-hour response time and 24/7 schedule, Sev-B with a 4-hour response time and 24/7 schedule, and Sev-C with an 8-hour response time during business hours.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Help topics were created under Manage → Help Topics to categorize incoming tickets. Topics included Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, and Other.
</p>
<br />
