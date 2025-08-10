# 🍫 Chocolatey (perso) – Packages & Automation Powerhouse 🚀

**Gestionnaire de paquets Windows inspiré de `apt-get`**, rapide à prendre en main, basé sur NuGet et PowerShell. Automation, packaging, installation fluide — tout y est.

---

![💻 OS](https://img.shields.io/badge/OS-Windows-blue)  
![💬 Langage](https://img.shields.io/badge/Language-PowerShell%20%7C%20NuGet-yellow)  
![✅ Status](https://img.shields.io/badge/Status-Lab%20Ready-success)  
![📜 Licence](https://img.shields.io/badge/License-Apache%202.0-blue)  

---

## 📑 Table des matières
1. [📜 Présentation](#-présentation)  
2. [✨ Fonctionnalités](#-fonctionnalités)  
3. [⚙️ Installation & Usage](#️-installation--usage)  
4. [📦 Packaging interne](#-packaging-interne)  
5. [🔒 Sécurité & précautions](#-sécurité--précautions)  
6. [🤝 Contribuer](#-contribuer)  
7. [📄 Licence](#-licence)

---

## 📜 Présentation
Chocolatey est un **gestionnaire de paquets CLI pour Windows**, s’appuyant sur PowerShell et NuGet.  
Il permet d’installer, mettre à jour et désinstaller facilement des applications, zips, scripts et exécutables.  
➡️ [Documentation officielle](https://docs.chocolatey.org/en-us/getting-started)

---

## ✨ Fonctionnalités
- 📥 **Installation rapide** de logiciels (MSI, EXE, ZIP, scripts)  
- 🔄 **Mises à jour automatiques** via CLI (`choco upgrade`)  
- 📦 **Packaging léger** basé sur NuGet  
- 🛠 **Intégration DevOps** : scripts d’infra & automatisation  
- 🏢 **Support entreprise** (Pro/Business)

---

## ⚙️ Installation & Usage

```powershell
# 🛠 Installation classique (PowerShell admin)
Set-ExecutionPolicy Bypass -Scope Process -Force
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# 🚀 Utilisation basique
choco install <package>
choco upgrade <package>
choco uninstall <package>
