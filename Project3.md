<h1>Project 3</h1>



<h2>Description</h2>
This project is about how to install Windows 11 OS in Virtual Box
<br />


<h2>Languages</h2>

- <b>CLI</b> 

<h2>Environments Used </h2>

- <b>Virtual Box</b>
- <b>Windows 11</b>

<h2>Program walk-through:</h2>

<!-- <p align="center"> --!>

1 - Launch Virtual Box and Select New <br />
<img width="860" alt="Open Virtual Box and Select New" src="https://user-images.githubusercontent.com/103763124/195167872-6db1d5da-7c75-47a7-a805-bea7c4826c24.png">
<br />
2 - Give your VM a Name <br/>
<img width="860" alt="Give your VM a Name" src="https://user-images.githubusercontent.com/103763124/195167736-fd8c86b5-dc09-4c2f-8ea6-4fc45d7cbeed.png">
<br />
3 - Give your VM a suitable amount of RAM <br/>
<img width="860" alt="Give your VM a suitable amount of RAM" src="https://user-images.githubusercontent.com/103763124/195167755-26f4c21a-a43d-438c-8b04-7026eaccfb51.png">
<br />
4 - Give your VM a suitable amount of Space <br/>
<img width="860" alt="Give your VM a suitable amount of Space" src="https://user-images.githubusercontent.com/103763124/195167773-9704b2fe-5d99-4744-a465-6cfa7ace83cb.png">
<br />
5 - Select your VM and click on Settings then System and Deselect Enable EFI <br/>
<img width="860" alt="Deselect Enable EFI" src="https://user-images.githubusercontent.com/103763124/195167689-2a20a5df-3df9-4fb5-8243-c0634599365a.png">
<br/>
6 - Now select Storage and add your Windows 11 ISO <br/>
<img width="860" alt="Open Storage Settings and add ISO file" src="https://user-images.githubusercontent.com/103763124/195167801-7463ccf6-9bee-4829-9ba4-b971cafd52b4.png">
7 - Start your VM. When you get to the Windows Setup page close the setup <br />
<img width="707" alt="Click the X button " src="https://user-images.githubusercontent.com/103763124/195167669-360b2ebd-ac40-4c45-b5aa-dc52d19f52be.png">
<br />
8 - Then select Repair your computer <br/>
<img width="707" alt="Select Repair " src="https://user-images.githubusercontent.com/103763124/195167959-6dff0dc1-fd9c-4ea9-b014-8e68ed34c878.png">
<br />
9 - Select troubleshoot <br/>
<img width="707" alt="Select Troubleshoot" src="https://user-images.githubusercontent.com/103763124/195167983-ea522fab-e4d7-45f1-8987-f883e8cce98e.png">
<br />
10 - Select Command Prompt <br/>
<img width="707" alt="Select Command Prompt" src="https://user-images.githubusercontent.com/103763124/195167897-2d5d1be5-2e2d-4086-a19d-a8f9fe926b70.png">
<br />
11 - Type regedit and press enter <br/>
<img width="707" alt="Type regedit" src="https://user-images.githubusercontent.com/103763124/195168010-56c2b81e-f752-4263-95a7-c20b6498a710.png">
<br/>
12 - Expamd HKEY_LOCAL_MACHINE and then expand SYSTEM <br/>
<img width="707" alt="Select Local Machine then Systems" src="https://user-images.githubusercontent.com/103763124/195167927-e5bbfc79-60a4-4666-8b4d-1bc606ebb135.png">
<br />
13 - Select and expand the setup folder <br />
<img width="707" alt="Select the Setup folder" src="https://user-images.githubusercontent.com/103763124/195167976-0bb5029b-aef8-49cc-a35b-12f913a103e7.png">
<br />
14 - Right click on the Setup folder and select New then Key and called it LabConfig <br/>
<img width="707" alt="Add LabConfig Folder" src="https://user-images.githubusercontent.com/103763124/195167596-eb809f05-884e-481b-b859-0ad60648599d.png">
<br />
15 - Inside the LabConfig folder right click and create New DWORD (32-bit) Value and call it BypassTPMCheck <br/>
<img width="707" alt="Add BypassTPMCheck" src="https://user-images.githubusercontent.com/103763124/195167588-eb897e51-dc90-4531-ab5c-57b96dd784f9.png">
<br />
16 - Select the BypassTPMCheck and change its Vaule to 1 <br/>
<img width="707" alt="Change BypassTPMCheck vaule to 1" src="https://user-images.githubusercontent.com/103763124/195167642-00882f86-423f-4588-b165-4761dfe7616b.png">
<br />
17 - Also Inside the LabConfig folder right click and create NEW DWORD (32-bit) Vaule and call it BypassSecureBootCheck <br/>
<img width="707" alt="Add BypassSecureBootCheck" src="https://user-images.githubusercontent.com/103763124/195167561-597d2977-a59a-4d31-b7fe-d7349871b885.png">
<br/>
18 - Select the BypassSecureBootCheck and change its Vaule to 1 <br/>
<img width="707" alt="Change BypassSecureBootCheck vaule to 1" src="https://user-images.githubusercontent.com/103763124/195167627-45c2e8ce-0c68-45e9-8e1c-be142d55c3ec.png">
<br />
19 -  Close the regedit window and type setup in the CMD and press enter<br />
<img width="707" alt="Exit the regedit and Type Setup" src="https://user-images.githubusercontent.com/103763124/195167721-374394c7-e6fd-4b1a-b6a9-8f9740bbc915.png">
<br />
20 - When the Windows Setup shows up again select Next <br/>
<img width="707" alt="Select Next" src="https://user-images.githubusercontent.com/103763124/195167944-6d82f2ca-577f-4302-8b2d-1f4b1d55d031.png">
<br />
21 - Agree to the terms and select Next <br/>
<img width="707" alt="Agree to the terms and Select Next" src="https://user-images.githubusercontent.com/103763124/195167610-798106af-75ca-4665-b7bf-577707b02b39.png">
<br />
22 - Select Custom <br/>
<img width="707" alt="Select Custom" src="https://user-images.githubusercontent.com/103763124/195167913-67a63986-245c-4e92-ba74-41a11e26c340.png">
<br />
23 - Select Next <br/>
<img width="707" alt="Click Next" src="https://user-images.githubusercontent.com/103763124/195167654-a1e0b6cc-b706-4500-8e34-cb039d2824f7.png">
<br/>
24 - Let the installation complete <br/>
<img width="707" alt="Let the installation complete" src="https://user-images.githubusercontent.com/103763124/195167791-614e6bb0-1fc7-41fe-902d-4a32928c9c4b.png">
25 - After the installation completes and the VM restarts complete the rest of the insalltion to your preference <br/>
<img width="707" alt="Select yes and contiune the installation" src="https://user-images.githubusercontent.com/103763124/195167998-b148e960-a952-414b-8555-1983e3c5d843.png">
<br/>
26 - After the VM restarts again you will have your Windows 11 OS installed <br/>
<img width="707" alt="Windows 11" src="https://user-images.githubusercontent.com/103763124/195168022-3d25fa38-95e5-4e41-9c09-ea5298b27eab.png">
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
