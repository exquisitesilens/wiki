#Git step for step

1. Full installer for official Git for Windows 1.8.3 [http://code.google.com/p/msysgit/downloads/list](http://code.google.com/p/msysgit/downloads/list)
2. Download TortoiseGit 1.8.5.0 (64 Bit) [tortoisegit](http://code.google.com/p/tortoisegit/wiki/Download?tm=2)
3. Clone Powershell from [https://github.com/dahlbyk/posh-git](https://github.com/dahlbyk/posh-git) - A set of PowerShell scripts which provide Git/PowerShell integration.
4. Configure Powershellprofil (Microsoft.PowerShell_profile.ps1)

   `# Load posh-git example profile`

   `. (([System.IO.Path]::GetDirectoryName($PROFILE)) + '\Poshgit\profile.example.ps1')`

so on: 
[7 Useful Git Tips for Beginners](http://sixrevisions.com/web-development/git-tips/)
