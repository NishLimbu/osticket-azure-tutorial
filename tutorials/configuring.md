## osTicket Administrative Setup

After completing the installation, follow these steps to configure osTicket for production use. This includes setting up users, agents, teams, roles, departments, and SLAs.

---

### Step 1: Log in to the Admin Panel
1. Open your browser and navigate to the public IP address of your VM.
2. Log in using the administrator credentials set during the osTicket installation.

---

### Step 2: Create Users
1. Go to **Users > Add New User**.
2. Fill out the user's details:
   - **Name**: Enter the full name.
   - **Email**: Provide the user's email address.
3. Click **Add User**.
4. Repeat for additional users.

![Add New User](./images/admin-users.png)

---

### Step 3: Configure Agents
1. Navigate to **Agents > Add New Agent**.
2. Enter the agent's details:
   - **Name**: Enter the full name.
   - **Email**: Provide the agent's email address.
   - **Username**: Set a username for the agent.
3. Assign the agent to a department.
4. Set their permissions and access levels.
5. Click **Add Agent**.

![Add New Agent](./images/admin-agents.png)

---

### Step 4: Create Teams
1. Go to **Agents > Teams** and click **Add New Team**.
2. Name the team (e.g., "IT Support Team").
3. Assign agents to the team.
4. Save the configuration.

---

### Step 5: Define Roles
1. Navigate to **Agents > Roles**.
2. Create a new role (e.g., "Support Manager").
3. Set permissions for each module (e.g., Tickets, Knowledgebase).
4. Assign roles to agents.

---

### Step 6: Configure Departments
1. Go to **Admin Panel > Departments** and click **Add Department**.
2. Name the department (e.g., "Customer Support").
3. Configure department settings, such as email templates and ticket auto-assignment.
4. Save the department.

![Department Configuration](./images/admin-departments.png)

---

### Step 7: Set Up Service Level Agreements (SLAs)
1. Navigate to **Admin Panel > Manage > SLA Plans**.
2. Click **Add New SLA Plan**.
3. Define the SLA parameters:
   - **Name**: (e.g., "Standard SLA").
   - **Response Time**: Set response and resolution time limits.
   - **Schedule**: Define working hours.
4. Save the SLA Plan.

![SLA Configuration](./images/admin-sla.png)

---

### Step 8: Test Your Configuration
1. Log in as a user and create a ticket.
2. Log in as an agent and manage the ticket.
3. Ensure all roles, SLAs, and departments function as expected.

---

## Resources
- [osTicket Documentation](https://docs.osticket.com/)
- [Example SLA JSON](./resources/example-sla.json)
- [Example Department JSON](./resources/example-department.json)
