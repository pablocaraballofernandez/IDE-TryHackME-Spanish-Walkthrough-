<div align="center">

#  TryHackMe - IDE 

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

Guía completa y detallada de la máquina **IDE** de TryHackMe, documentando todo el proceso de penetración desde el reconocimiento inicial hasta la obtención de privilegios root. Este repositorio incluye explicaciones técnicas paso a paso, comandos utilizados y conceptos de seguridad aplicados.

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

### Clonar el Repositorio
```bash
git clone https://github.com/tuusuario/ide-writeup.git
cd ide-writeup
