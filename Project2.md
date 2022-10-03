<h1>Project 2</h1>

<!-- [YouTube Demonstration](https://www.youtube.com/watch?v=w2bKo3xiEUU) --!>

<h2>Description</h2>
This project is about adding Users in Active Directory and creating Groups. Then adding Users to those Groups all by using different methods.
<br />


<h2>Languages</h2>

- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows Server 2022</b>
- <b>Active Directory User and Computers</b>

<h2>Program walk-through:</h2>

<!-- <p align="center"> --!>
1 - Adding a User in Active Directory Users and Computers <br/>
•	Open Server Manger <br/>
•	Select Tools from the top right and open Active Directory Users and Computers <br/>
•	Expand your domain from the left side <br/>
•	Right click on the Users folder. Select New then User <br/>
•	After creating your User click next. Create a Password select next then finish <br/>
<img width="700" alt="Adding User to AD" src="https://user-images.githubusercontent.com/103763124/185810364-691e2a22-be55-4c8d-988e-fb34c3f5c766.png"/>
<br />
<br />
2 - Adding a User in Active Directory Users and Computers using PowerShell <br/>
•	Search PowerShell from the taskbar then right click on PowerShell and run as admin <br/>
•	Run the following commands <br/>

New-ADUser -Name “Define the User’s Full Name”
-GivenName “Define User’s First Name” 
-Surname “Define the User’s Surname”
-SamAccountName “Define User’s Login Name”
-UserPrincipalName “Users login Name followed by a @ sign and your Domain Name” 
-Path “Define the OU Path” 
-AccountPassword(Read-Host -AsSecureString “Type a Password for the User”) -Enabled $true <br/>
<img width="700" alt="Adding User in AD using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810380-8f61aa72-2956-4cee-bcf7-249f41fde56e.png"/>
<br />
<br />
3 - Creating Groups in Active Directory Users and Computers <br/>
•	Open Server Manger <br/>
•	Select Tools from the top right and open Active Directory Users and Computers <br/>
•	Expand your domain from the left side <br/>
•	Right click on the Users folder. Select New then Group <br/>
•	Create a Group and select OK <br/>
<img width="700" alt="Creating Groups in AD" src="https://user-images.githubusercontent.com/103763124/185810415-30420f5d-f4cb-469c-9dd2-e2731d97fa10.png">
<br />
<br />
4 - Creating Groups in Active Directory Users and Computers using PowerShell <br/>
•	Search PowerShell from the taskbar right click on PowerShell and run as admin <br/>
•	Run the following commands <br/>

New-ADGroup -Name “Group’s Name”
-Description “Description of the Group”
-GroupScope DomainLocal 
(*The -GroupScope parameter can be set to DomainLocal, Global, or Universal depending on your company*) <br/>
<img width="700" alt="Adding Group in AD using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810433-05277324-b4c0-4c01-a0fd-97f42e2560ca.png"/>
5 - Adding a User to a Group in Active Directory Users and Computers <br/>
Method 1 <br/>
•	Open Server Manger
•	Select Tools from the top right and open Active Directory Users and Computers <br/>
•	Expand your domain and from the left side <br/>
•	Double Click on the Users Folder <br/>
•	On the right side double click on the User’s name <br/>
•	Select (Member of) from the top bar<br/>
•	Select Add <br/>
•	Enter the Group’s name and select OK <br/>
•	Select Apply and then OK <br/>
<img width="700" alt="Adding a User to a Group Method 1" src="https://user-images.githubusercontent.com/103763124/185810453-1b064ce4-94ed-439f-a9b9-722606026c81.png">
Method 2 <br/>
•	Open Server Manger <br/>
•	Select Tools from the top right and open Active Directory Users and Computers <br/>
•	Expand your domain and from the left side <br/>
•	Double Click on the Users Folder <br/>
•	On the right side double click on the Group’s name <br/>
•	Select (Members) from the top bar <br/>
•	Select Add <br/>
•	Enter the User’s name and Select OK <br/>
•	Select Apply and then OK <br/>
<img width="700" alt="Adding a User to a Group Method 2" src="https://user-images.githubusercontent.com/103763124/185810459-547934fe-aa60-4cab-bf31-940d615e37d1.png">
6 - Adding a User to a Group in Active Directory Users and Computers using PowerShell <br/>
•	Search PowerShell from the taskbar right click on PowerShell and run as admin <br/>
•	Run the following commands <br/>
   
Add-ADGroupMember -Identity “Enter the Group’s Name”
-Members “Enter the Member’s login Name” 
(*To add multiple Members use a common after the First Member and type the next Member after it*) <br/>
<img width="700" alt="Adding User to a Group using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810461-6b25bd03-7515-4f75-84f0-da5ee0cd791e.png">
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
