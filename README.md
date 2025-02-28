<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
 <p>This repository is based on an osTicket lab I completed during my IT Course Careers training. I will walk through the step-by-step process I learned for the post-installation setup of osTicket.

This is a great opportunity to gain a deeper understanding of the administrative side of osTicket, including how priorities are assigned. We will be creating different roles, departments, teams, agents (workers), and users (customers). Additionally, I will demonstrate how to configure SLAs (Service Level Agreements) and set up Help Topics.</p>
</p>
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h1><strong>osTicket Post Installation Setup</strong></h1>
<ul>
<h2>Step 1</h2>
<li>Open Azure and make sure your VM is running then open RDP and log into your VM</li>
<li>Now open your Admin/Analyst Login Page:
 <strong>http://localhost/osTicket/scp/login.php</strong></li>
</ul> 

<h2>Step 2</h2>
<p align="center"><strong>Unerstanding Agent Panel VS Admin Panel and Configuration Within</strong></p> 
<h3>Roles</h3>
<ul>
<li>Adding a <strong>Supreme Admin</strong> role</li> 
<li>Configiuring roles for grouping permissions.</li>
<li>Admin Panel > Agents > Roles</li>
</ul>
<p>
<img src="https://i.imgur.com/b7DudaQ.png" alt="roles 1"/>
</p>
<p>
<img src="https://i.imgur.com/VGg9IpO.png" alt="roles 2"/>
</p> 
<img src="https://i.imgur.com/CknWBS8.png" alt="role 3"/> 
<img src="https://i.imgur.com/PGWx2wJ.png" alt="role 4"/> 
<p>The Supreme Admin in osTicket has the highest level of control, allowing full access to system settings, user management, and security configurations. They can override restrictions, customize workflows, manage plugins, and perform critical tasks like backups and updates. This role ensures centralized control over the helpdesk system, preventing unauthorized changes while maintaining smooth operations.</p>
<h3>Departments</h3>
<ul>
 <li>Configuring ticket visibility for diffrent departments</li>
 <li>We have to create a <strong>SysAdmin</strong> to oversee operations</li>
</ul>
<p>
 <img src="https://i.imgur.com/fs58u2y.png" alt="dep 1"/> 
 <ul>
  <li>Admin > Agents > Departments</li>
  <li>Type SysAdmin for name:</li>
 </ul>
</p>
<img src="https://i.imgur.com/fS1MKJm.png" alt="dep 2"/>
<h3>Teams</h3>
<ul>
 <li>I'll be adding <strong>Online Banking</strong> to organizing and streamline customer support or internal operations related to online banking services. </li>
 <li>To assign agents from diffrent departments</li>
</ul>
<p>
 <img src="https://i.imgur.com/uSVfNe9.png" alt="Teams 1"/>
 <ul>
  <li>Admin Panel > Agent > Teams</li>
  <li>Then click <strong>Add New team</strong></li>
 </ul>
</p>
<img src="https://i.imgur.com/awHBMXN.png" alt="Teams 2"/> 
<h3 style=" color: red;">Allow Anyone to Create Tickets</h3>
<ul>
 <li>Go to Admin Panel > Settings > User Preferences.</li>
 <li>Under Allow ticket creation by set it to Anyone (this allows even non-registered users to create tickets).</li>
 <li>Also make sure to <strong>UNCHECK</strong> "Registration Required"</li>
</ul>
<img src="https://i.imgur.com/eVCTyQY.png" alt="regir-req"> 
<h3>Agents</h3>
<ul>
 <li>Admin Panel > Agents > Add New</li>
 <li>Jane as part of the department of <strong>SysAdmins</strong></li>
 <li>John as part of the department of <strong>Support</strong></li>
</ul>
<p>Jane</p>
<img src="https://i.imgur.com/RSGjWig.png" alt="agentsJ1">
<img src="https://i.imgur.com/lJP1Qt0.png" alt="agentsJ2">
<p>I'am also going to add Jane to the Online Banking Team</p>
<img src="https://i.imgur.com/y6mNA5A.png" alt="agentsJ3">
<img src="https://i.imgur.com/5YWBGoi.png" alt="agentsJ4">
<p>Here I'll just add John as a Support Agent</p>
<img src="https://i.imgur.com/UUqYFEE.png" alt="agentsJn1"> 
<h3>Users</h3>
<ul>
 <li>Agent Panel > Users > Add New</li>
 <li>I'll be creating <Strong>Tim</Strong> as our user</li> 
</ul>
<img src="https://i.imgur.com/Iv5nzSL.png" alt="userTim">
<h3>SLA Service Level Agreement</h3>
<p> Used to define and enforce the response and resolution times for tickets. They help ensure that support teams meet certain expectations for responding to and resolving customer inquiries or issues. SLAs are an essential tool for maintaining service quality and managing customer satisfaction.</p>
<ul>
 <li>Admin Panel > Manage > SLA</li>
 <li>Sev-A with a Grace Period of: 1 hour, and a Schedule of: 24/7</li>
 <li>Sev-B with a Grace Period of: 4 hours, and a Schedule of: 24/7</li>
 <li>Sev-C with a Grace Period: 8 hours, During Business Hours</li> 
</ul>
<img src="https://i.imgur.com/Hv1QOvL.png" alt="SLAs">
<img src="https://i.imgur.com/FdWSZ0N.png" alt="SLAs2">
<h3>Help Topics</h3>
<p>Last configuration so that users can create tickets.</p>
<ul>
 <li>Admin Panel > Manage > Help Topics</li>
 <li>Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, Other</li>
</ul>
<img src="https://i.imgur.com/LaC2fc3.png" alt="helpTopics">
<img src="https://i.imgur.com/R5d2dZq.png" alt="helpTopics2">




