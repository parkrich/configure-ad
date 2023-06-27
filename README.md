<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Configuring Active Directory Within Azure VMs</h1>
This briefly goes over the creation of Active Directory in a Cloud Environment.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Windows Server and Windows 10 VMs
- Connect both VMs
- Install Active Directory in Windows Server
- Create Admin and "Employee" accounts in AD
- Join Windows 10 to Windows Server IP
- Setup Remote Desktop for Powershell generated users in Windows Server
- Create users for Windows 10 access in Windows Server

<h2>Deployment and Configuration Steps</h2>

<p>
This is PowerShell creating several thousand random users for the Active Directory database. Powershell code was pulled from pre-coded source.
</p>

![image](https://github.com/parkrich/configure-ad/assets/137697108/3eb302eb-0b68-4470-af97-78e947200dc4)
<br />

<p>
Observing the random users in Active Directory uunder the "_Employees Organizational Unit. These will be the users that can access the Windows 10 machine under the domain forest created specifically for this lab, mydomain.com.
</p>

![image](https://github.com/parkrich/configure-ad/assets/137697108/755c1fa4-7e39-4145-b6da-c2cd323122ec)
<br />

<p>
One of the thousands of randomly generated users I selected to test to see if they can access the Windows 10 machine.
</p>

![image](https://github.com/parkrich/configure-ad/assets/137697108/e8bc599d-6709-4e9a-b60d-a19d495967b3)

<p>Confirmation of successful login as new user...</p>

![image](https://github.com/parkrich/configure-ad/assets/137697108/6b75893a-4b77-409c-a0a5-4c235ea36b9a)
<br />
