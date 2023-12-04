# Chocolatey
Archive zip des scripts d'installation de Chocolatey et installation de logiciels automatisés

# Pre-requis
CMD et Powershell

# Installation
- avec PowerShell (avec les droits administrateur)

```bash  
Set-ExecutionPolicy Bypass -Scope Process -Force; Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')) -ErrorAction Stop
powershell choco feature enable -n allowGlobalConfirmation
MKDIR c:\scripts
CD \scripts
wget https://github.com/sbeteta42/chocolatey/archive/refs/heads/main.zip -OutFile "C:\scripts\chocolatey.zip"
Expand-Archive -LiteralPath C:\scripts\chocolatey.zip -DestinationPath "C:\scripts\" -Force
cd chocolatey-main 
Expand-Archive -LiteralPath C:\scripts\chocolatey-main\chocolatey.zip -DestinationPath "C:\scripts\chocolatey-main" -Force
cd chocolatey
.\install_soft_client_windows.bat
```
