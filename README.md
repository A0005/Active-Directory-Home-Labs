PROJECT 1

•	Download and Install Virtual Box

•	Download and Install Windows 2022 Standard Edition with Desktop Experience on Virtual Box

•	Rename the Server to a suitable name

•	Download and Install Chrome or Brave browser or you can stick with Microsoft Edge

•	Download and Install Unified Communications Managed Api 4.0 Runtime

•	Download and Install Microsoft Visual C++ 2013 Redistributable (x64)

•	Install Active Directory Domain Services and Promote the Server to become a Domain Controller

•	Change Ethernet Settings for IPV4 and IPV6 to obtain DNS Automatically

•	Download Exchange 2019 and upload it using Virtual Box



•	Installation Commands for Exchange Server 2019

   1-	Open PowerShell and run as Administrator
   
   2-	Change into the directory that Exchange Server was uploaded to for example type d: 
   
   3-	Type Install-WindowsFeature RSAT-ADDS
   
   5-	Preparing Schema Type .\setup /PrepareSchema /IAcceptExchangeServerLicenseTerms
   
   6-	Preparing Active Directory Type .\setup /Preparead /IAcceptExchangeServerLicenseTerms /OrganizationName:"COMPANY"
   
   7-	Preparing Domain Type .\setup /Preparedomain /IAcceptExchangeServerLicenseTerms



•	Open File Explorer and Right Click on the Exchange drive and click Install or Run Program from media

•	Click on the start menu and expand the Exchange Folder Sever 2019 and select Exchange Administrative Center and login


<img width="555" alt="Windows Server 2022 Installation" src="https://user-images.githubusercontent.com/103763124/185809379-a26cfde3-0f2a-4b1e-80a4-356b90f220b2.png">

