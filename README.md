**<h1>osTicket - Post-Install Configuration</h1>**

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Add new Roles, Departments, and Teams.
- Add new Agents (workers), and allow anyone to create tickets.
- Add new Users (customers).
- Configure SLA.
- Configure Help Topics.

<h2>Configuration Steps</h2>
1. Log in to Osticket as an administrator using http://localhost/oSticket/scp/settings.php 
<p>
<p align="center">
<img src="https://i.imgur.com/kUrs7eu.png" alt="osTicket logo"/>
</p>

2. Create New Agents
   - While in the Admin Panel, click the "Agents" tab
   - Click "Add New Agent".
   - Give the agent a name, email, username, and password.
   - Click the "Access" tab
   - Assign agent to the "System Administrators" department.
   - Giveb "Supreme Admin" role.
   - Add agent to the "Level II Support" team.
<p>
<img src="https://i.imgur.com/v8tEAPM.png" height="90%" width="70%" alt=""/>
</p>
<p>

3. Create Departments
<img src="https://i.imgur.com/SiufMUN.png" height="70%" width="70%" alt=""/>
</p>

4. Add Roles:
   - "Agents" -> "Roles".
   - Next, click "Add New Role"
   - Name the role "Supreme Admin".
   - Click the "Permissions" tab
   - Enable every permission
   - Add the role.
</p>
<p>
<img src="https://i.imgur.com/4RJZyFV.png" height="70%" width="70%" alt=""/>
</p>
<p>

5. Add New Customers/Users
   - Log in as agent using (http://localhost/osTicket/scp/login.php)
   - Click "Users" tab
   - Click "Add User".
   - Give the user a name and an email.
   - Click "add user"
   - Repeat to add more users
   - Allow anyone to create a ticket -> While in the Admin panel, click settings -> Users -> then under "Authentication Settings" make sure "Require registration and login to create tickets" is unchecked.
</p>
</p>
<p>
<img src="https://i.imgur.com/TpUfuYH.png" height="70%" width="70%" alt=""/>
</p>
<p>

6. Configure SLA.
   - In the "Admin Panel" -> click "Manage"
   - Click the "SLA" tab
   - Click "Add New SLA Plan"
   - Name it "SEV-A", make the schedule "24/7", and make the grace period "1 hour".
   - Add another plan, name it "SEV-B", make the schedule "24/7", and make the grace period "4 hours".
   - Add one more plan, name it "SEV-C", make the schedule "Monday - Friday 8 am - 5 pm", and make the grace period "8 hours".
</p>
<br />
<p>
<img src="https://i.imgur.com/hPZ3I5I.png" height="70%" width="70%" alt=""/>
</p>
<p>
  
7. Configure Help Topics.
   - In the "Admin Panel" click "Manage"
   - Click "Help Topics"
   - Click "Add New Help Topic".
   - Name the topic "Business Critical Outage", and leave the parent topic as is.
   - Repeat the steps and create more help topics named "Personal Computer Issues", "Equipment Request", and "Password Reset".
     
     </p>
<br />
<p>
<img src="https://i.imgur.com/7J6wCEp.png" height="70%" width="70%" alt=""/>
</p>
<p>
8. The osTicket post-installation steps are now complete.
<br />
