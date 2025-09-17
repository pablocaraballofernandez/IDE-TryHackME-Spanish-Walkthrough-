<div align="center">

#  TryHackMe - IDE Machine Writeup

</div>
<div align="center">

![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)

[![Writeup](https://img.shields.io/badge/Writeup-Complete-success?style=for-the-badge)](https://github.com/tuusuario/ide-writeup)
[![Difficulty](https://img.shields.io/badge/Difficulty-Easy%2FMedium-yellow?style=for-the-badge)](https://tryhackme.com/room/ide)
[![Platform](https://img.shields.io/badge/Platform-Linux-orange?style=for-the-badge)](https://tryhackme.com)

</div>

##  Descripción

Writeup completo y detallado de la máquina **IDE** de TryHackMe, documentando todo el proceso de penetración desde el reconocimiento inicial hasta la obtención de privilegios root. Este repositorio incluye explicaciones técnicas paso a paso, comandos utilizados y conceptos de seguridad aplicados.

##  Objetivos de la Máquina

- [x] Reconocimiento y enumeración de servicios
- [x] Explotación de servicio FTP con acceso anónimo
- [x] Ataque de fuerza bruta a aplicación web
- [x] Explotación de RCE en Codiad (CVE-2018-14009)
- [x] Movimiento lateral entre usuarios
- [x] Escalada de privilegios mediante sudo misconfiguration
- [x] Obtención de flags user.txt y root.txt

## 🛠 Tecnologías y Herramientas

### Herramientas de Pentesting
- **Nmap** - Escaneo de puertos y servicios
- **Burp Suite** - Interceptación y fuerza bruta
- **Netcat** - Reverse shells
- **Python** - Ejecución de exploits
- **SecLists** - Wordlists para fuerza bruta

### Servicios Vulnerables
- **vsFTPd 3.0.3** - Acceso anónimo mal configurado
- **Codiad 2.8.4** - Remote Code Execution
- **Systemd** - Service misconfiguration

##  Contenido del Writeup

### 1. Reconocimiento
- Escaneo completo de puertos con Nmap
- Identificación de servicios vulnerables
- Enumeración de versiones

### 2. Acceso Inicial
- Explotación de FTP anónimo
- Descubrimiento de credenciales
- Fuerza bruta en Codiad
- RCE mediante CVE-2018-14009

### 3. Post-Explotación
- Técnica de Staged Reverse Shell
- Upgrade a TTY interactiva
- Movimiento lateral www-data → drac

### 4. Escalada de Privilegios
- Análisis de permisos sudo
- Explotación de systemd service
- Manipulación de archivos de configuración
- Obtención de shell root

##  Quick Start

### Clonar el Repositorio
```bash
git clone https://github.com/tuusuario/ide-writeup.git
cd ide-writeup
