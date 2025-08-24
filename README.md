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
1. Configure roles and permissions through the 'Admin' tab. 

If it says 'Agent' at the top right, you will know you are on the admin tab.   ~  <img width="150" height="35" alt="image" src="https://github.com/user-attachments/assets/ee72bbc2-1067-4133-aaa0-cc21dfcec087" />

<p>  
<img width="442" height="293" alt="image" src="https://github.com/user-attachments/assets/619d7001-7801-45d3-a58e-ddebff59d826" />
<p> 
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
<img width="438" height="206" alt="image" src="https://github.com/user-attachments/assets/44dfa4b6-3323-4883-913e-2e785d31a117" />

<p>
  
- Go to the **Admin Panel**. 

  
- Click on **Agents** > **Departments**.
  
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
<img width="440" height="65" alt="image" src="https://github.com/user-attachments/assets/7d037f62-1c4b-4d5e-b7a9-9b37aa01b406" />


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
<img width="440" height="281" alt="image" src="https://github.com/user-attachments/assets/db084bd2-3b15-4062-a6bb-6d1d8f1073e7" />

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
<img width="440" height="397" alt="image" src="https://github.com/user-attachments/assets/1c4b2c1c-559c-4758-9fb1-46b8bea6049d" />

<p>
Steps to Configure Agents:

- Navigate to the **Admin Panel**.
   
- Click on **Agents** in the sidebar menu.
  
- Choose an existing agent to edit, or click **Add New Agent**.
  
- Enter the agent’s details:
  
   - **Full Name**
   - **Email Address**
   - **Username** and **Password**
   - **Primary Department** (determines initial ticket access)
     
- Assign a **Role**:
  
   - Roles define what the agent can see and do in the system (e.g., Admin, Support Staff).
     
- (Optional) Assign the agent to one or more **Teams** for collaborative ticket handling.
  
- Click **Save Changes** to apply the configuration.

> 💡 Use roles and departments strategically to control access and responsibilities across your support team.
<p>
6. Configuring SLA Plans in osTicket
<p> 
SLA (Service Level Agreement) Plans define the expected response and resolution times for tickets. They help prioritize support and measure performance.
<p>
<img width="442" height="270" alt="image" src="https://github.com/user-attachments/assets/ef532308-2b56-40a3-9a8a-0982735a5296" />
<p>

#### Steps to Configure SLA Plans:

- Go to the **Admin Panel**.
  
- Click on **Manage** > **SLA Plans**.
  
- Click **Add New SLA Plan**.
  
- Fill in the following fields:
  
   - **Name** – e.g., "Standard", "Priority Support"
   - **Grace Period** – time allowed to respond or resolve (in hours)
   - **Schedule** – choose when the SLA applies (business hours, weekends, etc.)
     
- Click **Save Changes**.

> 💡 You can assign SLA Plans to Help Topics, Departments, or Tickets directly for automated prioritization.
> <p>
7. Configure Help Topics
8. <p>
