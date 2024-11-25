<h1>Create-AD-users-using-powershell-commands</h1>
<p>This tutorial outlines how to create Active Directory users using Windows powershell commands instead of the GUI.<br /></p>

<p>1. To create a domain user using PowerShell command, this command is used: "New-ADUser Username". In this project, I used Katy Perry as user’s name.</p>
<p align="center"><img src="https://i.imgur.com/bpydNCe.png" height="50%" width="50%"/>

<p>2. Because any account created is disabled by default until a password is set and account enabled, so I will assign a password to the account I just created by using this command "Set-ADAccountPassword -Identity Katy.Perry" and also enable this account with this command prompt; "Enable-ADAccount -Identity Katy.Perry". </p>
<p align="center"><img src="https://i.imgur.com/VdGWClw.png" height="50%" width="50%"/>
<p align="center"><img src="https://i.imgur.com/8nZzIy5.png" height="50%" width="50%"/>

<p>3. To create another user, we will repeat the same process.  Powershell command; "New-ADUser Username". This second user’s name will be Lucas Jones. </p>
<p align="center"><img src="https://i.imgur.com/md8aO7u.png" height="50%" width="50%"/>

<p>4. Because any account created is disabled by default until a password is set and account enabled, so I will assign a password to the account I just created by using this command "Set-ADAccountPassword -Identity Lucas.Jones" and also enable this account with this command prompt; "Enable-ADAccount -Identity Lucas.Jones".</p>
<p align="center"><img src="https://i.imgur.com/2BkVzaJ.png" height="50%" width="50%"/>
<p align="center"><img src="https://i.imgur.com/oUv0oCE.png" height="50%" width="50%"/>

<p>5. To view all the new domain users created, I used this command prompt; "Get-ADUser -Filter * -Properties samAccountName | select samAccountName".</p>
<p align="center"><img src="https://i.imgur.com/hjSYE1A.png" height="50%" width="50%"/>
