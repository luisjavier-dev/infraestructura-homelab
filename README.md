# 🏠 Infraestructura de Homelab

Infraestructura doméstica personal centrada en redes, virtualización y servicios autoalojados.

## 🧠 Resumen

Este proyecto representa mi infraestructura doméstica, diseñada para simular un entorno empresarial pequeño.  

Objetivos principales:
- Segmentación y seguridad de red
- Virtualización de servicios
- Automatización y escalabilidad
- Experimentación con sistemas domóticos

---

## 🖥️ Hardware

- HP ProDesk 400 G6 Mini
  - Intel i5-10500T
    - 6 núcleos
    - 12 subprocesos
    - Hyper-Threading
  - 24 GB RAM
  - SSD 500 GB

---

## 🌐 Arquitectura de Red

- Router del ISP en modo bridge
- Host Proxmox
- VM OPNsense (firewall y routing)
- Switch gestionable (TP-Link SG608E)
- Punto de acceso WiFi (Huawei AX3)

**Diagrama de red:**  
![Diagrama de red](diagrams/Diagrama.png)


---

## 🌐 Rendimiento
- Iperf en LAN
  
![Diagrama de red](diagrams/RendimientoLAN.png)

- Test de velocidad con SpeedTest Ethernet
  
![Diagrama de red](diagrams/TestWanEth.png)

- Test de velocidad con SpeedTest WiFi
  
![Diagrama de red](diagrams/TestWanWiFi.png)
---

## 🔐 Redes

- Reglas de firewall con OPNsense
- Acceso VPN mediante WireGuard

---

## 🧩 Virtualización (Proxmox)

### Máquinas Virtuales

- OPNsense (Firewall y VPN)
- Ubuntu Server (Samba NAS en RAID1)
- Ubuntu Server (Jarvis AI – en desarrollo)

### Contenedores (LXC)

- Stack de automatización doméstica:
  - Broker MQTT
  - Node-RED
  - Dashboard web
  - Web Server (Apache)

**Arquitectura Proxmox:**  
![Arquitectura Proxmox](diagrams/proxmox-architecture.png)

---

## 🏠 Automatización Domótica

- Comunicación basada en MQTT
- Dispositivos ESP8266, ESP32 y NodeMCU
- Flujos Node-RED para automatización

**Flujos Node-RED:**  
![Flujos Node-RED](diagrams/node-red-flows.png)

---

## 🗂️ Estructura de carpetas del repo

```text
homelab-infrastructure/
│
├── README.md
├── diagrams/                 # Diagramas de red, VMs y flujos Node-RED
├── configs/                  # Archivos de configuración de ejemplo
│   ├── opnsense/
│   ├── mqtt/
│   └── apache/
└── docs/                     # Documentación extra (manuales, notas)
