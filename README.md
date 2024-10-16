# admin
admin


``
C:\WINDOWS\system32\runas.exe /profile /env /user:%userdomain%\a-%username% powershell
``

After running above command, run this other commands:

``
Set-PSReadLineOption -HistorySaveStyle SaveNothing
``

``
Set-PSReadLineOption -HistorySavePath "C:\Temp\PowerShellHistory.txt"
``

### Okay now lets remote into remote computer

``Enter-PSSession``

When it prompt for computername, please enter the hostname only.

Now, lets check who's member of Administrators group

``Get-LocalGroupMember -Name Administrators``

Now, lets add user into Administrators group

``Add-LocalGroupMember -Name Admnistrators -Member usernameHERE``
