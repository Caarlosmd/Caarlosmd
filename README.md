# 💻 Carlos Martinez Diaz
### Futuro Técnico Superior en ASIR | Especialista en Sistemas y Redes

---

## 👤 Sobre mí
¡Hola! Soy un estudiante de **Administración de Sistemas Informáticos en Red (ASIR)**. Mi objetivo es garantizar que las infraestructuras tecnológicas sean seguras, eficientes y escalables. Me encanta investigar nuevas soluciones de código abierto y optimizar servicios en entornos Linux.

* 🔭 **Estado actual:** Cursando 1º de ASIR y desarrollando proyectos de red.
* 🌱 **Aprendiendo:** Automatización con `Ansible` y despliegue de contenedores con `Docker`.
* 🛠️ **Filosofía:** "Si tienes que hacerlo más de dos veces, automatízalo".

---

## 🛠️ Stack Tecnológico (Habilidades)

| Área | Tecnologías |
| :--- | :--- |
| **Sistemas** | `Debian/Ubuntu Server`, `Windows Server 2022`, `Active Directory` |
| **Redes** | `Cisco Packet Tracer`, `Protocolos TCP/IP`, `VLANs`, `VPN` |
| **Seguridad** | `Firewalls (iptables)`, `Análisis de Logs` |
| **Servicios** | `DNS`, `DHCP`, `FTP`, |
| **Virtualización** | `VMware Workstation`, `VirtualBox`, `Proxmox` |

---

## 📂 Proyectos y Prácticas Realizadas

### 🛠️ Configuración de Dominio.
Despliegue de un Dominio con endurecimiento de seguridad, restringiendo accesos mediante ACL y OUs.


## 🎯 Objetivo Profesional

Mi meta principal es la especialización técnica y el crecimiento profesional:
* 🚩 **A corto plazo:** Realizar mis prácticas (FCT) en entornos de **Infraestructura Cloud** o **Ciberseguridad**.
* 🚀 **Visión de futuro:** Convertirme en *Administrador de Sistemas Senior*.
* 🛠️ **Especialización:** Alta disponibilidad y continuidad de negocio.

## 📬 Contacto
¿Te interesa mi perfil o quieres colaborar en algún proyecto? ¡Hablemos!

* 📧 **Email:** caarlosmdd@gmail.com
* 💼 **LinkedIn:** linkedin.com/in/carlos-martinez
* 📍 **Ubicación:** Murcia, España (Disponible para remoto)

#!/bin/bash
# Script para comprobar el estado de un servicio crítico
SERVICE="apache2"

if systemctl is-active --quiet $SERVICE; then
    echo "El servicio $SERVICE está funcionando correctamente."
else
    echo "ALERTA: El servicio $SERVICE está caído. Intentando reiniciar..."
    sudo systemctl start $SERVICE
fi
