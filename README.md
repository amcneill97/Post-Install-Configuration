<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This guide walks through the post-install setup and configuration of osTicket, an open-source support ticketing platform.<br />


<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles & Permissions

- Configure Departments

- Configure Teams
   
- Tweak settings to allow anyone to create tickets

- Configure Agents

- Configure SLA and Help Topics

<h2>Configuration Steps</h2>

<p>
1. Configure roles and permissions through the 'Admin' tab. If it says 'Agent' at the top right, you will know you are on the admin tab.
<p>  
<img width="445" height="163" alt="image" src="https://github.com/user-attachments/assets/bb2a030a-d6c8-489e-a153-d1b051637444" />

To control what agents can see or access in osTicket:

- Navigate to the **Admin Panel**.
- Click on **Agents**.
- Go to **Roles**.
- Open the **Permissions** tab.
- Adjust the settings as needed to manage agent access.

> 💡 Use roles and permissions carefully to maintain security and appropriate access levels within your support system.
<p>
2. Configure Departments through the 'Departments' tab.
<p>
<img width="442" height="411" alt="image" src="https://github.com/user-attachments/assets/99bc5db2-d0ae-4544-85d9-97b6f1b5d1c3" />
<p>
  
- Go to the **Admin Panel**.
  
- Click on **Departments** in the navigation menu.
- Select an existing department to edit, or click **Add New Department**.
- Fill in the required fields:
   - **Name** – e.g., "Technical Support", "Billing"
   - **Email** – the email address associated with this department
   - **Department Manager** – the primary agent responsible
- Configure access permissions and settings based on your workflow.
- Click **Save Changes** to apply the updates.

> 💡 Departments can be used to route tickets automatically and define which agents have access to certain types of requests.

<p>
3. Teams are used to group agents for collaboration and ticket assignment across departments. To set up or manage teams:
<p>
<img width="439" height="140" alt="image" src="https://github.com/user-attachments/assets/0a237bbe-bf1d-444b-9a0b-c84f99ad8a1c" />


- Navigate to the **Admin Panel**.
- Click on **Teams** in the navigation menu.
- Select an existing team to edit, or click **Add New Team**.
- Fill in the team details:
   - **Name** – e.g., "Level 2 Support", "Escalations Team"
   - **Team Lead** – the agent responsible for overseeing the team
   - **Members** – select agents to include in the team
- Define the team's access level and assign them to specific departments if needed.
- Click **Save Changes** to apply the configuration.

> 💡 Teams are useful for organizing agents by expertise or responsibility, especially when tickets span multiple departments or require escalation.

<p>
4. Unrestrict ticket creation so anyone can submit tickets
<p>
<img width="441" height="314" alt="image" src="https://github.com/user-attachments/assets/8436071e-e179-4fd5-bb7c-83090a6719ad" />
<p> 
By default, osTicket may restrict ticket creation to registered users or authenticated agents. To allow anyone to create tickets (e.g., via the web form or email):

- Go to the **Admin Panel**.
- Click on **Settings** > **User Settings**.
- Under the **Registration** or **User Authentication** section:
   - Ensure that **"Require registration/login to open tickets"** is **unchecked**.
- Click **Save Changes** to apply the new settings.

Optional:  
To accept tickets via email from unregistered users:

- Go to **Emails** > **Email Settings**.
- Make sure you have at least one email address configured and enabled for **ticket creation**.
- Ensure your mail fetching (POP/IMAP) is working so incoming emails generate tickets.

> ⚠️ Allowing unrestricted ticket creation may increase the risk of spam. Consider enabling CAPTCHA or using a spam filter.
<p>
5. Configure Agents


<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
