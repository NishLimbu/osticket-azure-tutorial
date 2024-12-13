## osTicket Ticket Management in a Lab Environment

This section demonstrates the process of creating, triaging, and resolving mocked tickets in osTicket to simulate real-world support workflows.

---

### Step 1: Create Mocked Tickets
1. Log in as a user.
2. Navigate to the **Open a New Ticket** page.
3. Fill out the ticket form:
   - **Name**: Enter a mock user name.
   - **Email**: Provide a mock email address.
   - **Help Topic**: Select a topic (e.g., "IT Support").
   - **Subject**: Describe the issue (e.g., "Unable to connect to VPN").
   - **Message**: Provide details about the issue.
4. Submit the ticket.

![Create Ticket](./images/create-ticket.png)

---

### Step 2: Triage Tickets
1. Log in as an agent or admin.
2. Go to the **Tickets** tab to view the list of open tickets.
3. Assign tickets to the appropriate agent or department:
   - Select the ticket.
   - Click **Assign to Agent/Team** and choose the responsible party.
4. Update the ticket’s status (e.g., "In Progress").

![Triage Ticket](./images/triage-ticket.png)

---

### Step 3: Resolve Tickets
1. Access the ticket assigned to you.
2. Review the details provided by the user.
3. Add a response to the ticket:
   - Go to the **Post Reply** section.
   - Provide a solution or request additional details.
4. Mark the ticket as resolved:
   - Update the ticket status to **Closed**.
5. (Optional) Add internal notes for future reference.

![Resolve Ticket](./images/resolve-ticket.png)

---

### Step 4: Validate Workflow
1. Log back in as a user and verify that the issue has been resolved.
2. Test notifications and response times to ensure SLA compliance.

---

## Resources
- [Example Ticket Data](./resources/example-ticket-data.json)
