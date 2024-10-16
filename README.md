# admin
admin


``
C:\WINDOWS\system32\runas.exe /profile /env /user:%userdomain%\a-%username% powershell
``

After running above command, run this other commands:

``
Set-PSReadLineOption -HistorySaveStyle SaveNothing
Set-PSReadLineOption -HistorySavePath "C:\Temp\PowerShellHistory.txt"
``
