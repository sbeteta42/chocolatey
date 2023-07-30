# chocolatey
Archive zip des scripts d'installation de Chocolatey et installation de logiciels automatisés

# pre-requis
Installer GIT sous votre client Windows

# Installation
- avec CMD (avec les droits administrateur)

```bash  
MKDIR c:\scripts
CD scripts
git clone https://github.com/sbeteta42/chocolatey
Expand-Archive -LiteralPath C:\scripts\chocolatey.zip -DestinationPath "C:\scripts\" -Force
.\install_chocolatey.bat
.\install_soft_client_windows.bat
