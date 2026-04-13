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
<img width="619" height="199" alt="Screenshot 2026-04-13 at 3 28 49 PM" src="https://github.com/user-attachments/assets/bc4aae96-afd3-4034-9425-4ac41254d1c5" />
</p>
<p>
Roles were created in the Admin Panel under Agents → Roles to define permission levels. A “Supreme Admin” role was established to grant full system access and control over configurations.
</p>
<br />

<p>
<img width="943" height="203" alt="Screenshot 2026-04-13 at 12 45 54 PM" src="https://github.com/user-attachments/assets/d47b06c7-bf6d-4640-bdd7-af3afa755527" />
</p>
<p>
Departments were set up in the Admin Panel under Agents → Departments to control ticket visibility and organization. A “SysAdmins” department was created to handle system-related support requests.
</p>
<br />

<p>
<img width="950" height="146" alt="Screenshot 2026-04-13 at 12 45 34 PM" src="https://github.com/user-attachments/assets/b8afaa5c-d225-43e7-b830-f58288899fdd" />
</p>
<p>
Teams were configured under Agents → Teams to allow collaboration across departments. An “Online Banking” team was created to group agents from different departments working on similar tasks or services.
</p>
<br />
  
<p>
<img width="943" height="203" alt="Screenshot 2026-04-13 at 12 45 54 PM" src="https://github.com/user-attachments/assets/8686d777-3b9d-4993-b75c-9032844b1034" />
  <img width="952" height="181" alt="Screenshot 2026-04-13 at 12 45 24 PM" src="https://github.com/user-attachments/assets/a8d3f0d4-59b0-46b1-871e-dafc6c2b6e3c" />

</p>
<p>
Agents (support staff) were added through the Admin Panel under Agents → Add New. Two agents were created: Jane, assigned to the SysAdmins department, and John, assigned to the Support department.
</p>
<br />

<p>
<img width="951" height="201" alt="Screenshot 2026-04-13 at 12 46 12 PM" src="https://github.com/user-attachments/assets/fb8e4b90-2b7f-419d-870b-6b870e60fc57" />
</p>
<p>
End users (customers) were added through the Agent Panel under Users → Add New. Two users, Karen and Ken, were created to simulate customer interactions within the help desk system.
</p>
<br />

<p>
<img width="952" height="236" alt="Screenshot 2026-04-13 at 12 45 07 PM" src="https://github.com/user-attachments/assets/b1b25c28-4b9e-4f32-94c5-ea361912ec37" />
</p>
<p>
Service Level Agreements (SLAs) were configured under Manage → SLA in the Admin Panel. Three SLA levels were created: Sev-A with a 1-hour response time and 24/7 schedule, Sev-B with a 4-hour response time and 24/7 schedule, and Sev-C with an 8-hour response time during business hours.
</p>
<br />

<p>
<img width="945" height="506" alt="Screenshot 2026-04-13 at 12 45 00 PM" src="https://github.com/user-attachments/assets/ae0b3f04-1773-4022-b379-fe2300eac380" />
Help topics were created under Manage → Help Topics to categorize incoming tickets. Topics included Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, and Other.
</p>
<br />
