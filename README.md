# Chocolatey
Archive zip des scripts d'installation de Chocolatey et installation de logiciels automatisés

# Pre-requis
PowerShell et CMD

# Installation
- Vous devez lancer PowerShell ou Windows Terminal en tant qu'ADMINISTRATEUR ! La méthode recommandée consiste à cliquer avec le bouton droit sur le menu Démarrer et à sélectionner (PowerShell en tant qu'administrateur Windows 10 - Terminal Windows en tant qu'administrateur Windows 11)

```bash  
Set-ExecutionPolicy Bypass -Scope Process -Force
Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')) -ErrorAction Stop
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
