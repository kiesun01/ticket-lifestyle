<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle </h1>
This repository offers a detailed guide on the lifecycle of tickets within the osTicket help desk system. It encompasses the entire ticket process, from creation to resolution, which includes:<br />
<br />
Part 1: Ticket Creation (3 steps) <br />
Part 2: Answering tickets and troubleshooting Permissions (8 steps)<br />
Part 3: Assigning, escalating, and closing tickets (9 steps)<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure: Utilized for Virtual Machines and compute resources
- Remote Desktop: For managing and accessing the virtual machines.
- Internet Information Services (IIS): Acts as the web server hosting osTicket.
  
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Active Subscription (Creation of Reasearch Group, VMs, Virtual Networks, Subnets)
- Enable Internet Information Services(IIS)
- PHP Manager
- Rewrite Manager
- C++ Redistributbal
- MySQL Server
- Install osTicket
- Assigning Permissions
- osTicket
- Supreme Admin: jerry
- Agents: cameron.jones and jane.doe


<h2>Part 1 (Ticket Creation) Steps: 1 - 3 </h2>

![image](https://github.com/user-attachments/assets/feb810ca-6544-416f-b5da-8e13b39c7057)
<p>
Step 1: Click open a New Ticket
</p>
<br />

![image](https://github.com/user-attachments/assets/b8c066a9-f058-4657-89a3-55a604f421b7)
![image](https://github.com/user-attachments/assets/2dc76476-ea74-4b9a-bc6c-7a5daa08618a)
<p>
Step 2: Fill out the form with client and ticket information. Click Create Ticket. (ex: Ken Smith)
</p>
<br />

![image](https://github.com/user-attachments/assets/2c48f7f1-9272-456d-ac7f-b5e98587476a)
![image](https://github.com/user-attachments/assets/c7ce031a-b54e-4343-8db9-8eb3e8b97db8)
![image](https://github.com/user-attachments/assets/484606d0-c36e-4421-bc81-00462277bd82)
<p>
Step 3: Add several more client form follow the previous step. (ex. Ashley Walker, Tyler Howard)
</p>
<br />

<h2>Part 2: (Answering Tickets and troubleshooting Permissions) Steps: 1 - 8</h2>

![image](https://github.com/user-attachments/assets/468c8718-cd1c-4802-8809-6c5902488e43)
<p>
Step 1: Help desk will navigate to http://localhost/osTicket/scp/login.php to respond to tickets. Enter credentials
</p>
<br />

![image](https://github.com/user-attachments/assets/bb3a4545-bcc8-4901-b7aa-f89d9d35f758)
<p>
Step 2: We know from Step 1, that 3 tickets have been created. We cannot see them currently becausee agent Cameron does not have permissions. 
</p>
<br />

![image](https://github.com/user-attachments/assets/4661edb5-c503-4476-abdf-0533d4044d28)
<p>
Step 3: Log Out as Cameron and log in as Admin: jerry
</p>
<br />

![image](https://github.com/user-attachments/assets/b6f26ab7-c0a2-40dd-8b4e-7d7a5b74ef6f)
<p>
Step 4: This is agent panel where we can view tickets. Click on ticket to see department (ex: When are we getting a hardware refresh)
</p>
<br />

![image](https://github.com/user-attachments/assets/013f3c9b-76e8-49a6-a364-abad8d57b80c)
<p>
Step 5: We need to give agent Cameron permissions to the Department: Support, so he can respond to support tickets.
</p>
<br />

![image](https://github.com/user-attachments/assets/39c90c7c-da2b-435f-8c4c-529ec96d1545)
<p>
Step 6: Click Admin Panel -> Agents. This is a list of all Agents. Notice how Cameron is NOT in the Support department. Click Cameron Jones -> Access
</p>
<br />

![image](https://github.com/user-attachments/assets/711184bf-fa15-4efa-a088-cb7061b4c23f)
<p>
Step 7: We can change his primary department, or add extended access permissions to the Support. Add as Supreme Admin, to the Support -> Save
</p>
<br />

![image](https://github.com/user-attachments/assets/81aba0e5-d1a6-48a7-80ed-aea2e24b1a96)
<p>
Step 8: Log out as admin. Log back in as Cameron. Agent Cameron with Supreme Admin for Support can now view/respond the tickets. FYI: Supreme Admin was used as a random hypothetical, however it is not best practice to grant Admin to Agents that don't really need it. It would be better to grant them access only to what they need to perform their duties.
</p>
<br />
<br />
<br />


<h2>Part 3: (Assigning, escalating tickets, and closing) Steps: 1 - 9</h2>

![image](https://github.com/user-attachments/assets/b1233b87-a8d2-4745-8202-0763ba0bce07)
<p>
Step 1: Click the ticket (Entire system not working)
</p>
<br />

![image](https://github.com/user-attachments/assets/3f7f8560-cb11-4d47-a82a-3494dc745ccd)
![image](https://github.com/user-attachments/assets/1b5e343b-90d6-4171-af57-2ee4d6a58979)
<p>
Step 2: This is a high-stake business impacting incident, therefore it make sense to change Priority to Emergency. Changed Assigned To: Cameron (whoever the escalation engineer is or queue manager). Also we change the Service Level Agreement to the most urgent: SEV-A
</p>
<br />

![image](https://github.com/user-attachments/assets/25a9a12d-a38c-4374-b55c-961a1dd28c3c)
<p>
Step 3: If Support is not equipped to handle the ticket, it may also be a good idea to escalate the department as well (ex: System Administrators)
</p>
<br />

![image](https://github.com/user-attachments/assets/0ee28308-a945-4e09-ac10-4a90e1d02b54)
<p>
Step 4: View of ticket history.
</p>
<br />

![image](https://github.com/user-attachments/assets/3c6d2420-3ff0-476c-b317-423d0c24c667)
<p>
Step 5: In this case, we leave the Ticket Status: Open, until it is resolved.
</p>
<br />

![image](https://github.com/user-attachments/assets/d0343154-0e40-4d2c-9626-1c51c40b9a2a)
<p>
Step 6: Ticket has now been properly assigned to agent Cameron Jones, and Priority has been escalated
</p>
<br />

![image](https://github.com/user-attachments/assets/7331c30e-3ff8-4c20-8726-c86fef78ff95)
![image](https://github.com/user-attachments/assets/a1176d95-5317-44fc-804c-76c24dbe6ed5)
<p>
Step 7: A response is posted to declare the ticket solved. Change ticket status to Resolved.
</p>
<br />

![image](https://github.com/user-attachments/assets/474fa3b7-1083-4e67-8a03-0482c73cf3a1)
<p>
Step 8: After resolving the ticket, it is removed from the ticket tab. If we want to see the ticket, click Closed
</p>
<br />

![image](https://github.com/user-attachments/assets/4ff49491-53d7-4dfd-b3d8-e41aeaa5f3bb)
<p>
Step 9: This tab tells us important information like when a ticket is closed, and by whom.
</p>
<br />
