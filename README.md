# Chocolatey
Archive zip des scripts d'installation de Chocolatey et installation de logiciels automatisés

# Pre-requis
CMD et Powershell

# Installation
- avec PowerShell (avec les droits administrateur)

```bash  
MKDIR c:\scripts
CD \scripts
wget https://github.com/sbeteta42/chocolatey/archive/refs/heads/main.zip -OutFile "C:\scripts\chocolatey.zip"
Expand-Archive -LiteralPath C:\scripts\chocolatey.zip -DestinationPath "C:\scripts\" -Force
cd chocolatey-main\ 
Expand-Archive -LiteralPath C:\scripts\chocolatey-main\chocolatey.zip -DestinationPath "C:\scripts\chocolatey-main" -Force
cd chocolatey\ 
.\installChocolatey.cmd
.\install_soft_client_windows.bat
