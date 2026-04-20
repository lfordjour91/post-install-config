<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - osTicket Setup</h1>
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
 <b>Step 1: Access The System</b>
 <ul>
<li>Admin Login Page:</li>
  <ul>
<li><a href="http://localhost/osTicket/scp/login.php">Admin Login</a></li>
  </ul>
<li>End User Portal:</li>
  <ul>
<li><a href="http://localhost/osTicket/">End User Portal</a></li>
  </ul>
 </ul>
</p>
<p>
<img width="619" height="199" alt="Screenshot 2026-04-13 at 3 28 49 PM" src="https://github.com/user-attachments/assets/bc4aae96-afd3-4034-9425-4ac41254d1c5" />
</p>
<br />

<p>
 <b>Step 2: Understand Admin Panel vs Agent Panel</b>
Before configuring anything, understand the difference:
<ul>
  <li>Admin Panel</li>
  <ul>
 <li>Used for system configuration</li>
 <li>Manage roles, departments, SLAs, settings</li>
  </ul>
 <li>Agent Panel</li>
  <ul>
 <li>Used by support staff (agents)</li>
 <li>Handle tickets, manage users, respond to issues</li>
  </ul>
</ul>
<p>
<img width="1920" height="1080" alt="Artboard 2" src="https://github.com/user-attachments/assets/0fae7a9a-1c03-4166-b743-9822e2589b83" />
</p>
<br />

<p>
 <b>Step 3: Configure Roles</b><br>
 Roles define what agents are allowed to do.
  
<p style="font-weight: 500;">Path:<br>
Admin Panel → Agents → Roles</p><br>
Actions:
<ol>
<li>Click “Add New Role”</li>
<li>Name the role: Supreme Admin</li>
<li>Assign full permissions (all checkboxes)</li>
</ol>
This role has complete control over the system.
<p>
<img width="1920" height="1080" alt="Artboard 3" src="https://github.com/user-attachments/assets/b712082e-e722-4a63-8f44-bd980af85e6b" />
</p>
<br />

<p>
 <b>Step 4: Configure Departments</b>
 Departments control ticket visibility and routing.
Path:
Admin Panel → Agents → Departments
Actions:
  <ol>
<li>Click “Add New Department”</li>
<li>Name: SysAdmins</li>
<li>Configure visibility (default settings are fine)</li>
  </ol>
Departments separate responsibilities (e.g., IT vs Support).
<p>
<img width="1920" height="1080" alt="Artboard 4" src="https://github.com/user-attachments/assets/e1a19b93-bd3e-4c5a-ba2a-c8c54974ee3c" />
</p>
<br />

<p>
 <b>Step 5: Configure Teams</b>
Teams allow agents from different departments to collaborate.
Path:
Admin Panel → Agents → Teams
Actions:
  <ol>
<li>Click “Add New Team”</li>
<li>Name: Online Banking</li>
<li>Add members from multiple departments</li>
  </ol>
💡 Useful for cross-functional issues.
<p>
<img width="1920" height="1080" alt="Artboard 5" src="https://github.com/user-attachments/assets/c54911ed-5c7e-48d0-86f7-aea532700ec6" />
</p>
<br />

<p>
 <b>Configure User Ticekt Permissions</b>
 Decide whether anyone can submit tickets.
Path:
Admin Panel → Settings → User Settings
Actions:
  <ul>
<li>UNCHECK: Unregistered users can create tickets</li>
<li>ENABLE: Require registration and login to create tickets</li>
  </ul>
💡 This ensures only verified users can submit requests.
<p>
<img width="1920" height="1080" alt="Artboard 6" src="https://github.com/user-attachments/assets/ce23a2c8-d494-4c43-965e-ce770724c965" />
</p>
<br />

<p>
 <b>Step 7:Congifure Agents</b>
 Agents are the workers handling tickets.
Path:
Admin Panel → Agents → Add New
Create the following:
Agent 1:
  <ul>
<li>Name: Jane</li>
<li>Department: SysAdmins</li>
  </ul>
Agent 2:
<ul>
<li>Name: John</li>
<li>Department: Support</li>
</ul>
<p>
<img width="1920" height="1080" alt="Artboard 7" src="https://github.com/user-attachments/assets/69d754b6-1436-438b-9df4-09c6cf1e9a1e" />
</p>
<br />

<p>
 <b>Configure Users</b>
Users are the people submitting tickets.
Path:
Agent Panel → Users → Add New
Create:
  <ul>
<li>Karen</li>
<li>Ken</li>
  </ul>
<p>
<img width="1920" height="1080" alt="Artboard 8" src="https://github.com/user-attachments/assets/8e2d23f2-3a5e-4aa3-b64a-3c89eb194880" />
</p>
<br />

<p>
 <b>Configure SLA</b>
 SLAs define response/resolution time expectations.
Path:
Admin Panel → Manage → SLA
Create:
Sev-A (High Priority)
  <ul>
<li>Grace Period: 1 hour</li>
<li>Schedule: 24/7</li>
  </ul>
Sev-B (Medium Priority)
      <ul>
<li>Grace Period: 4 hours</li>
<li>Schedule: 24/7</li>
      </ul>
Sev-C (Low Priority)
          <ul>
<li>Grace Period: 8 hours</li>
<li>Schedule: Business Hours</li>
          </ul>
💡 SLAs help prioritize urgent issues.
<p>
<img width="1920" height="1080" alt="Artboard 9" src="https://github.com/user-attachments/assets/197e4ed1-d125-4853-a1a5-988b3faf638e" />
</p>
<br />

<p>
 <b>Configure Help Topics</b>
 Help Topics guide users when creating tickets.
Path:
Admin Panel → Manage → Help Topics
Create:
  <ul>
<li>Business Critical Outage</li>
<li>Personal Computer Issues</li>
<li>Equipment Request</li>
<li>Password Reset</li>
<li>Other</li>
  </ul>
💡 These categorize tickets automatically.
<p>
 <img width="1920" height="1080" alt="Artboard 10" src="https://github.com/user-attachments/assets/9612008e-1fd1-4fb0-91f4-33e604578133" />
</p>
<br />

<p>
 <b> FINAL RESULTS</b>
 After completing this setup:
  <ul>
<li>Users can register and submit tickets</li>
<li>Tickets are categorized by help topics</li>
<li>Agents are assigned based on departments</li>
<li>SLAs enforce response times</li>
<li>Teams allow collaboration across departments</li>
  </ul>
<p>

</p>
<br />
