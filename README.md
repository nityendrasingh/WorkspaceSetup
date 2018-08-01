# WorkspaceSetup

1. Setup Powershell:
Open Powershell in administrator mode:
* Set-ExecutionPolicy RemoteSigned
* This is for figuring out location of profile script:<br>
PS C:\> $Profile.AllUsersAllHosts    =>    C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1 <br>
PS C:\> $Profile.AllUsersCurrentHost   =>    C:\Windows\System32\WindowsPowerShell\v1.0\Microsoft.PowerShell_profile.ps1 <br>
PS C:\> $Profile.CurrentUserAllHosts    =>    C:\Users\CurrentUser\Documents\WindowsPowerShell\profile.ps1 <br>
PS C:\> $Profile.CurrentUserCurrentHost   =>   C:\Users\CurrentUser\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1 <br> 

* cmd /c mklink C:\Windows\System32\WindowsPowerShell\v1.0\profile.ps1 $home\Dropbox\Workspace\profile.ps1

2. Setup Git:
* cmd /c mklink $home\.gitconfig $home\Dropbox\Workspace\gitconfig
* cmd /c mklink $home\.gitignore_global $home\Dropbox\Workspace\gitignore_global
