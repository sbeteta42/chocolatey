# Chocolatey
Archive zip des scripts d'installation de Chocolatey et installation de logiciels automatisés

# Pre-requis
CMD et Powershell

# Installation
- avec CMD (avec les droits administrateur)

```bash  
MKDIR c:\scripts
CD scripts
wget https://github.com/sbeteta42/chocolatey/chocolatey.zip
Expand-Archive -LiteralPath C:\scripts\chocolatey.zip -DestinationPath "C:\scripts\" -Force
.\installChocolatey.cmd
.\install_soft_client_windows.bat
