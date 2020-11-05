# W10_login_edge_launch
PowerShell script that'll launch Chromium-Edge at login (not unlock)

<img src="https://api.iconify.design/mdi:powershell.svg?color=blue&height=24"/>


I created this ps1 - PowerShell - script for work use, but decided to push it here at GitHub so anyone can have it.


I set it up at Group Policy via 'Edit Group Policy'.


User Configuration > Windows Settings > Scripts (Logon/Logoff) > Logon > PowerShell Scripts > Add


I set 'For this GPO, run scripts in the following order:' as 'Run Windows PowerShell scripts last'.


This is really simple PowerShell script that'll launch only Chromium-based Edge (tho, you can modify it to launch pretty much any application).


Script relies on `Start-Process`-cmdlet so you are required to add `-FilePath` for every application you want to start with this script.


This is used as-is if you're going to use [login_applaunch](https://github.com/RedFox-Development/W10_login_applaunch) to launch some PWAs on login.
