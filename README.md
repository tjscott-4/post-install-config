<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

---

### **Step 1: Access osTicket Panels**

**Instructions:**
- **Admin/Analyst Login Page:** `http://localhost/osTicket/scp/login.php`  
- **End-User Portal:** `http://localhost/osTicket`  
- Verified access to both **Agent Panel** (for staff) and **Admin Panel** (for system configuration).

📘 **Why this matters:**  
Understanding the difference between the two panels is essential for managing workflows and support escalation.

🧠 **Skills demonstrated:**  
Application administration, user interface navigation, system role distinction.

<img width="1038" height="508" alt="image" src="https://github.com/user-attachments/assets/5ccd2f2a-fa0e-4578-a533-d7983ac9d250" />
Agent Panel

<img width="964" height="431" alt="image" src="https://github.com/user-attachments/assets/d486f383-ded9-4538-9533-7e0b86eaaafc" />
Admin Panel

---

### **Step 2: Configure Roles**

**Instructions:**
- **Navigation:** Admin Panel → Agents → Roles  
- Created role: **Supreme Admin** (full administrative privileges).

📘 **Why this matters:**  
Roles define permissions and actions agents can perform in the helpdesk system.

🧠 **Skills demonstrated:**  
Role-based access control, user permission management.

<img width="962" height="420" alt="image" src="https://github.com/user-attachments/assets/35a47ef7-c034-4a5c-8be1-305bef51c595" />
<img width="956" height="481" alt="image" src="https://github.com/user-attachments/assets/4a38ef8f-996b-4b53-8caf-adda5e11fb46" />

---

### **Step 3: Configure Departments**

**Instructions:**
- **Navigation:** Admin Panel → Agents → Departments  
- Created department: **SysAdmins**  

📘 **Why this matters:**  
Departments define ticket routing and visibility, helping separate Help Desk, Networking, and SysAdmin tasks.

🧠 **Skills demonstrated:**  
Department configuration, workflow segmentation, access control.

<img width="960" height="412" alt="image" src="https://github.com/user-attachments/assets/51c3083f-1fc5-49f9-85e6-3fab36a8d907" />

---

### **Step 4: Configure Teams**

**Instructions:**
- **Navigation:** Admin Panel → Agents → Teams  
- Created team: **Online Banking**  
- Pulled agents from multiple departments for collaboration.

📘 **Why this matters:**  
Teams allow agents from different departments to collaborate on specific ticket categories or incidents.

🧠 **Skills demonstrated:**  
Team management, cross-department collaboration.

<img width="955" height="353" alt="image" src="https://github.com/user-attachments/assets/b1bedd88-c2d0-42af-85c9-8140f80bcffe" />

---

### **Step 5: Adjust User Registration and Ticket Settings**

**Instructions:**
- **Navigation:** Admin Panel → Settings → User Settings  
- **Unchecked:** “Unregistered users can create tickets.”  
- **Enabled:** “Require registration and login to create tickets.”

📘 **Why this matters:**  
Ensures that only registered users can submit tickets — improving tracking, accountability, and data integrity.

🧠 **Skills demonstrated:**  
User policy configuration, access control, data integrity.

<img width="960" height="432" alt="image" src="https://github.com/user-attachments/assets/1434b497-4f20-463c-9f02-cb499852b2ee" />

---

### **Step 6: Configure Agents (Help Desk Staff)**

**Instructions:**
- **Navigation:** Admin Panel → Agents → Add New  
- Added:
  - **Jane** → Dept: SysAdmins  
  - **John** → Dept: Support  

📘 **Why this matters:**  
Agents are responsible for resolving tickets; proper setup ensures efficient workload distribution.

🧠 **Skills demonstrated:**  
Staff account creation, department assignment, role management.

<img width="960" height="319" alt="image" src="https://github.com/user-attachments/assets/6a381e61-333b-4892-bcba-32b86608b8c5" />

---

### **Step 7: Configure Users (Customers)**

**Instructions:**
- **Navigation:** Agent Panel → Users → Add New  
- Added:
  - **Karen**
  - **Ken**

📘 **Why this matters:**  
Users represent customers or employees who submit tickets for technical support.

🧠 **Skills demonstrated:**  
User management, customer support setup, application configuration.

<img width="952" height="318" alt="image" src="https://github.com/user-attachments/assets/8a8f0785-2521-425d-83ce-d9c5db7ceb70" />
<img width="960" height="322" alt="image" src="https://github.com/user-attachments/assets/0c11f6e7-4926-4feb-8364-955726c3be69" />

---

### **Step 8: Configure SLA (Service Level Agreements)**

**Instructions:**
- **Navigation:** Admin Panel → Manage → SLA  
- Created:
  - **Sev-A** → 1-hour grace period (24/7)
  - **Sev-B** → 4-hour grace period (24/7)
  - **Sev-C** → 8-hour grace period (Business Hours)

📘 **Why this matters:**  
SLAs define response and resolution expectations based on ticket severity and business needs.

🧠 **Skills demonstrated:**  
SLA policy creation, IT service management, prioritization.

<img width="954" height="323" alt="image" src="https://github.com/user-attachments/assets/df810ba8-2572-4955-b2e2-5c9017efdd36" />
<img width="955" height="336" alt="image" src="https://github.com/user-attachments/assets/4f62b6e8-2c15-4669-84eb-9bcc5ed202dc" />
<img width="955" height="346" alt="image" src="https://github.com/user-attachments/assets/fadcd059-8bd8-402f-9a93-ba4bf42ff4d8" />


---

### **Step 9: Configure Help Topics**

**Instructions:**
- **Navigation:** Admin Panel → Manage → Help Topics  
- Created:
  - Business Critical Outage  
  - Personal Computer Issues  
  - Equipment Request  
  - Password Reset  
  - Other  

📘 **Why this matters:**  
Help Topics categorize incoming tickets to ensure proper routing to the right department or team.

🧠 **Skills demonstrated:**  
Ticket categorization, workflow optimization, process automation.

<img width="961" height="317" alt="image" src="https://github.com/user-attachments/assets/f0d80c2c-06a0-4052-abb5-9231ea8a9ea8" />
<img width="956" height="316" alt="image" src="https://github.com/user-attachments/assets/9f1ad284-db8f-49a2-a070-3e7257ccf37c" />
<img width="956" height="313" alt="image" src="https://github.com/user-attachments/assets/d0d172bd-3eea-4857-9857-156ca68d3b84" />
<img width="956" height="314" alt="image" src="https://github.com/user-attachments/assets/61abf3a0-2665-44c0-b10b-0482e9c0df54" />
<img width="957" height="309" alt="image" src="https://github.com/user-attachments/assets/12d6535b-222a-447a-8666-0a8ecc51926e" />
<img width="956" height="454" alt="image" src="https://github.com/user-attachments/assets/7bfa2eab-1167-4027-b3be-6300d771559b" />

---

✅ **End of Part 2: Post-Installation Configurations**

Next: [**Part 3 – Verification & Testing**](#part-3-verification--testing)
