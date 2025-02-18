<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
 <p>This repository is based on an osTicket lab I completed during my IT Course Careers training. I will walk through the step-by-step process I learned for the post-installation setup of osTicket.

This is a great opportunity to gain a deeper understanding of the administrative side of osTicket, including how priorities are assigned. We will be creating different roles, departments, teams, agents (workers), and users (customers). Additionally, I will demonstrate how to configure SLAs (Service Level Agreements) and set up Help Topics.</p>
</p>
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
