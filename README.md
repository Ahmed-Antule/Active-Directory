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
<img width="783" height="588" alt="3" src="https://github.com/user-attachments/assets/3776f8ab-eac3-4445-a09b-015e39f3cd6c" />


iii. Go to the "Confirmation" section and click "Install."
<img width="792" height="564" alt="Capture3" src="https://github.com/user-attachments/assets/9cdb70aa-0192-4397-9174-4c7dc971d16c" />

iv. Once the installation is complete, click on "Promote this server to a domain controller."
<img width="766" height="566" alt="Capture4" src="https://github.com/user-attachments/assets/5e4f38b6-795b-4594-b75c-39b724c5ee33" />

Why Click on "Promote This Server to a Domain Controller" in Active Directory Setup?
After installing Active Directory Domain Services (AD DS) on Windows Server 2019, the server needs to function as a Domain Controller (DC). Clicking "Promote This Server to a Domain Controller" is necessary because:

✅ Activates Directory Services – It enables the Active Directory database, allowing user authentication, group management, and security policies.
✅ Creates or Joins a Domain – It lets you either create a new domain (e.g., mycompany.local) or add the server to an existing domain.
✅ Manages Authentication & Security – The Domain Controller is responsible for verifying user logins, managing group policies, and securing access.
✅ Enables Group Policies (GPOs) – Once promoted, you can enforce security settings, software deployment, and administrative controls across the network.

Without promoting the server to a Domain Controller, the installed Active Directory services won't be functional, and the server will not manage users, groups, or policies effectively. 🚀

v. Click on "Add a New Forest" and enter the root domain name with the .local extension.
<img width="771" height="567" alt="Capture5" src="https://github.com/user-attachments/assets/27cfc6ff-905b-4d34-913d-78aec43a8dba" />





