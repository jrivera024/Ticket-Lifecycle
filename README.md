# Ticket-Lifecycle


In this lab, we will be creating tickets as end users.
Observing all the ticket properties and responding to them as help desk professionals


## Environments and Technologies Used
  - Microsoft Azure VM
  - Remote Desktop
  - Internet Information Service
  - osTicket

## Operating System Used
  - Window 10 Pro

## Ticket Lifecycle Stages

1.Ticket Creation / Logging
  - A ticket is created when a user reports an issue (via phone, email, chat, self-service portal, or auto-monitoring tool).
  - It’s recorded in the help desk system with details like user info, category, priority, and description.

2. Ticket Categorization & Prioritization
   - The help desk agent assigns the ticket to a category (e.g., hardware, software, network) and sets its priority (low, medium, high, critical).
   - This ensures the ticket is routed correctly and handled in the right order.

3. Ticket Assignment
  - The ticket is assigned to the appropriate technician or support group.
  - Escalation may occur if the issue is beyond the Tier 1 agent’s scope (e.g., moved to Tier 2/3).

4. Investigation & Diagnosis
   - The assigned technician reviews the ticket details, replicates the problem if possible, and investigates root causes.
   - May involve asking the user for more details, running diagnostics, or checking logs.

5. Resolution & Recovery
   - The technician applies a fix, workaround, or replacement.
   - The solution is documented in the ticket for reference.
   - The user is notified of the resolution.

6. Ticket Closure
   - Once the user confirms the issue is resolved (or the SLA requirement is met), the ticket is closed.
   - Closing includes final documentation, resolution code, and categorization for reporting.

7. Post-Closure Review (Optional)
   - Some organizations review closed tickets to identify recurring problems, improve knowledge base articles, or refine processes.
   - Helps with trend analysis and continuous improvement.


## Example: Online Banking system is down
### Ticket Creation
  - Create a ticket as an end-user

  <img width="943" height="323" alt="image" src="https://github.com/user-attachments/assets/4be97223-0e21-4fd4-928d-672faaf0ff41" />



### Ticket Categorization & Prioritization
  - Category: Application / Online Services
  - Subcategory: Online Banking Portal
  - Priority: Critical (High Business Impact)
  - SLA Target: 1 hour

  <img width="940" height="222" alt="image" src="https://github.com/user-attachments/assets/03d1f0bb-3019-48e6-8377-4f0feed05875" />


### Ticket Assignment
  - Assigned To: Application Support Team (Tier 2)
  - Escalation: Immediately escalated to Tier 3 Infrastructure since it affects all customers.

### Investigation & Diagnosis
  - Checked system monitoring: Portal server showing 100% CPU usage.
  - Database server unreachable from application server.
  - Verified with Network Team: Firewall logs show blocked DB traffic after last rule update.

### Resolution & Recovery
  - Network Team rolled back recent firewall change.
  - Database connectivity restored.
  - Online Banking portal accessible again (confirmed with test login).


### Ticket Closeure
  - User Confirmation: Bank Teller confirmed customers can log in successfully.
  - Resolution Code: Infrastructure Change / Firewall Misconfiguration.
  - Closure Time: 10:05 AM (35 minutes after logging).

    <img width="967" height="678" alt="image" src="https://github.com/user-attachments/assets/e178d745-21ea-4bb1-a529-52535fcc2f8b" />


### Post-Closure Review
  - Documented incident in Knowledge Base with troubleshooting steps.
  - Recommended Change Management Review to prevent future unapproved firewall rule changes.
  - Suggested setting up automatic application monitoring alerts tied to SLA response times.




