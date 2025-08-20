# Active-Directory

Windows Active Directory (AD) – Centralized Identity & Access Management
Windows Active Directory (AD) is a directory service developed by Microsoft that helps manage users, computers, and resources in a network. It is used in enterprise environments to provide centralized authentication, authorization, and security policies.

Key Features:
✅ User & Group Management – Centralized control over user accounts, groups, and permissions.
✅ Authentication & Authorization – Uses Kerberos and LDAP for secure user logins.
✅ Group Policy Management – Enforces security settings, software installations, and network configurations.
✅ Single Sign-On (SSO) – Users can access multiple applications with one set of credentials.
✅ Domain Services – Organizes network resources into domains, forests, and organizational units (OUs).

Why Use Active Directory?
🔹 Centralized Security – Manages access control across the organization.
🔹 Scalability – Supports thousands of users, devices, and applications.
🔹 Integration – Works with Microsoft services like Azure AD, Exchange, and SharePoint.
🔹 Improved Productivity – Users sign in once and access multiple resources without re-entering credentials.

Common Use Cases:
Enterprise IT Management – Controlling access to corporate networks and devices.
User Authentication & SSO – Secure logins for employees across applications.
Access Control & Security – Implementing policies for passwords, firewalls, and permissions.
Windows Active Directory is essential for managing and securing enterprise networks, ensuring efficient user and resource management. 🚀

Summary: Setting Up Active Directory on Windows Server 2019
In this project, I installed and configured Active Directory (AD) on Windows Server 2019 to manage users, groups, and computers within an organization. The steps include:

Installing Active Directory Domain Services (AD DS) on Windows Server 2019.
Creating an Organizational Unit (OU) to structure and manage directory objects.
Adding Users, Groups, and Computer OUs for efficient identity and access management.
This setup enables centralized authentication, authorization, and resource management, ensuring secure and efficient user administration within the domain. 🚀

Step - 1
i. Click on "Manage," then select "Add Roles and Features."
<img width="1366" height="705" alt="Capture1" src="https://github.com/user-attachments/assets/d070ef51-e353-4d6c-a656-d02bef555b81" />

ii. Go to "Server Roles," then select and install "Active Directory Domain Services (AD DS)."
<img width="790" height="573" alt="Capture2" src="https://github.com/user-attachments/assets/2cf6a616-8703-477e-ab13-b938f9d2d5c0" />
<img width="783" height="588" alt="3" src="https://github.com/user-attachments/assets/34d9a778-c873-48e7-82ed-2e1b79b2e130" />



iii. Go to the "Confirmation" section and click "Install."
<img width="800" height="562" alt="Capture3" src="https://github.com/user-attachments/assets/9f59c9e4-be31-4768-a909-2da5e8780cee" />


iv. Once the installation is complete, click on "Promote this server to a domain controller."
<img width="792" height="564" alt="Capture4" src="https://github.com/user-attachments/assets/ad1dc434-cc77-46f2-a8da-646c6c50000a" />


Why Click on "Promote This Server to a Domain Controller" in Active Directory Setup?
After installing Active Directory Domain Services (AD DS) on Windows Server 2019, the server needs to function as a Domain Controller (DC). Clicking "Promote This Server to a Domain Controller" is necessary because:

✅ Activates Directory Services – It enables the Active Directory database, allowing user authentication, group management, and security policies.
✅ Creates or Joins a Domain – It lets you either create a new domain (e.g., mycompany.local) or add the server to an existing domain.
✅ Manages Authentication & Security – The Domain Controller is responsible for verifying user logins, managing group policies, and securing access.
✅ Enables Group Policies (GPOs) – Once promoted, you can enforce security settings, software deployment, and administrative controls across the network.

Without promoting the server to a Domain Controller, the installed Active Directory services won't be functional, and the server will not manage users, groups, or policies effectively. 🚀

v. Click on "Add a New Forest" and enter the root domain name with the .local extension.
<img width="766" height="566" alt="Capture5" src="https://github.com/user-attachments/assets/20ced06d-f2cc-4b1c-9843-018efba6c420" />

vi. In the Domain Controller configuration, set and confirm the password for the domain.
<img width="771" height="567" alt="Capture6" src="https://github.com/user-attachments/assets/acf2d009-9778-4e5a-99e5-c3f2e2536ab0" />

vii. Click "Next" until you reach the prerequisites check, then click "Install."
<img width="769" height="568" alt="Capture7" src="https://github.com/user-attachments/assets/244f69b1-72db-4689-b21b-e8b06f6d9f5b" />

The VM will restart, and once it boots up, you will see that your domain has been successfully created.<br>
After logging in, you can view the installed components and configured settings within the Active Directory environment.
<img width="349" height="603" alt="10" src="https://github.com/user-attachments/assets/c96d8246-9984-443b-a30e-40f1eeba96db" />

Step - 2
i. Open "Active Directory Users and Computers" (ADUC).<br> <br>

ii. Right-click on your domain and select "New" > "Organizational Unit" to create a new OU.

What is an Organizational Unit (OU) in Active Directory? An Organizational Unit (OU) in Active Directory (AD) is a logical container used to organize and manage users, groups, computers, and other objects within a domain. It helps in structuring the directory to apply group policies and delegate administrative tasks efficiently

Example of OU Structure: 📂 Company.local (Root Domain) ├── HR (OU) → Users & Computers for HR ├── IT (OU) → Users & Computers for IT Team ├── Finance (OU) → Users & Computers for Finance

By using Organizational Units, businesses can structure their Active Directory efficiently, making it easier to manage users, devices, and policies. 🚀

ii. I have created an Organizational Unit (OU) named Company, which contains multiple sub-OUs for Users, Groups, Computers, and Servers.

iii. Steps to Create a New User

<img width="453" height="395" alt="Capture21" src="https://github.com/user-attachments/assets/5fffe3e4-bf33-48cc-8b57-55c9fdb4f455" />


Enter the password and select the checkbox below as per the company's policy.

<img width="447" height="387" alt="Capture22" src="https://github.com/user-attachments/assets/f237ed1a-21b6-413b-a7fb-99b4f2ce06fe" />
<img width="1366" height="413" alt="Capture23" src="https://github.com/user-attachments/assets/9a3e042e-ad29-4baf-88b6-7bddbee0b00a" />

















