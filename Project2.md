Project 2

1 - Adding a User in Active Directory Users and Computers

•	Open Server Manger

•	Select Tools from the top right and open Active Directory Users and Computers

•	Expand your domain from the left side

•	Right click on the Users folder. Select New then User

•	After creating your User click next. Create a Password select next then finish


<img width="869" alt="Adding User to AD" src="https://user-images.githubusercontent.com/103763124/185810364-691e2a22-be55-4c8d-988e-fb34c3f5c766.png">


2 - Adding a User in Active Directory Users and Computers using PowerShell

•	Search PowerShell from the taskbar then right click on PowerShell and run as admin

•	Run the following commands

New-ADUser -Name “Define the User’s Full Name”
-GivenName “Define User’s First Name” 
-Surname “Define the User’s Surname”
-SamAccountName “Define User’s Login Name”
-UserPrincipalName “Users login Name followed by a @ sign and your Domain Name” 
-Path “Define the OU Path” 
-AccountPassword(Read-Host -AsSecureString “Type a Password for the User”) -Enabled $true 


<img width="700" alt="Adding User in AD using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810380-8f61aa72-2956-4cee-bcf7-249f41fde56e.png">


3 - Creating Groups in Active Directory Users and Computers

•	Open Server Manger

•	Select Tools from the top right and open Active Directory Users and Computers

•	Expand your domain from the left side

•	Right click on the Users folder. Select New then Group

•	Create a Group and select OK


<img width="700" alt="Creating Groups in AD" src="https://user-images.githubusercontent.com/103763124/185810415-30420f5d-f4cb-469c-9dd2-e2731d97fa10.png">



4 - Creating Groups in Active Directory Users and Computers using PowerShell

•	Search PowerShell from the taskbar right click on PowerShell and run as admin

•	Run the following commands

New-ADGroup -Name “Group’s Name”
-Description “Description of the Group”
-GroupScope DomainLocal 
(*The -GroupScope parameter can be set to DomainLocal, Global, or Universal depending on your company*)


<img width="700" alt="Adding Group in AD using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810433-05277324-b4c0-4c01-a0fd-97f42e2560ca.png">


5 - Adding a User to a Group in Active Directory Users and Computers

Method 1

•	Open Server Manger

•	Select Tools from the top right and open Active Directory Users and Computers

•	Expand your domain and from the left side

•	Double Click on the Users Folder

•	On the right side double click on the User’s name

•	Select (Member of) from the top bar

•	Select Add

•	Enter the Group’s name and select OK

•	Select Apply and then OK


<img width="700" alt="Adding a User to a Group Method 1" src="https://user-images.githubusercontent.com/103763124/185810453-1b064ce4-94ed-439f-a9b9-722606026c81.png">


Method 2


•	Open Server Manger

•	Select Tools from the top right and open Active Directory Users and Computers

•	Expand your domain and from the left side

•	Double Click on the Users Folder

•	On the right side double click on the Group’s name

•	Select (Members) from the top bar

•	Select Add

•	Enter the User’s name and Select OK

•	Select Apply and then OK


<img width="700" alt="Adding a User to a Group Method 2" src="https://user-images.githubusercontent.com/103763124/185810459-547934fe-aa60-4cab-bf31-940d615e37d1.png">


6 - Adding a User to a Group in Active Directory Users and Computers using PowerShell

•	Search PowerShell from the taskbar right click on PowerShell and run as admin

•	Run the following commands
   
Add-ADGroupMember -Identity “Enter the Group’s Name”
-Members “Enter the Member’s login Name” 
(*To add multiple Members use a common after the First Member and type the next Member after it*)


<img width="700" alt="Adding User to a Group using PowerShell" src="https://user-images.githubusercontent.com/103763124/185810461-6b25bd03-7515-4f75-84f0-da5ee0cd791e.png">
