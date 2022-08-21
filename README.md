PROJECT 1

1	Download and Install Virtual Box

2	Download and Install Windows 2022 Standard Edition with Desktop Experience on Virtual Box

3	Rename the Server to a suitable name

4	Download and Install Chrome or Brave browser or you can stick with Microsoft Edge

5	Download and Install Unified Communications Managed Api 4.0 Runtime

5	Download and Install Microsoft Visual C++ 2013 Redistributable (x64)

7	Install Active Directory Domain Services and Promote the Server to become a Domain Controller

8	Change Ethernet Settings for IPV4 and IPV6 to obtain DNS Automatically

9	Download Exchange 2019 and upload it using Virtual Box



10	Installation Commands for Exchange Server 2019

   • Open PowerShell and run as Administrator
   
   • Change into the directory that Exchange Server was uploaded to for example type d: 
   
   • Type Install-WindowsFeature RSAT-ADDS
   
   • Install Required Roles Type Install-WindowsFeature NET-Framework-45-Features, RPC-over-HTTP-proxy, RSAT-Clustering, RSAT-Clustering-CmdInterface, RSAT-Clustering-Mgmt, RSAT-Clustering-PowerShell, Web-Mgmt-Console, WAS-Process-Model, Web-Asp-Net45, Web-Basic-Auth, Web-Client-Auth, Web-Digest-Auth, Web-Dir-Browsing, Web-Dyn-Compression, Web-Http-Errors, Web-Http-Logging, Web-Http-Redirect, Web-Http-Tracing, Web-ISAPI-Ext, Web-ISAPI-Filter, Web-Lgcy-Mgmt-Console, Web-Metabase, Web-Mgmt-Console, Web-Mgmt-Service, Web-Net-Ext45, Web-Request-Monitor, Web-Server, Web-Stat-Compression, Web-Static-Content, Web-Windows-Auth, Web-WMI, Windows-Identity-Foundation, RSAT-ADDS

   
   • Preparing Schema Type .\setup /PrepareSchema /IAcceptExchangeServerLicenseTerms
   
   • Preparing Active Directory Type .\setup /Preparead /IAcceptExchangeServerLicenseTerms /OrganizationName:"COMPANY"
   
   • Preparing Domain Type .\setup /Preparedomain /IAcceptExchangeServerLicenseTerms



11	Open File Explorer and Right Click on the Exchange drive and click Install or Run Program from media

12	Click on the start menu and expand the Exchange Folder Sever 2019 and select Exchange Administrative Center and login


<img width="555" alt="Windows Server 2022 Installation" src="https://user-images.githubusercontent.com/103763124/185809379-a26cfde3-0f2a-4b1e-80a4-356b90f220b2.png">

