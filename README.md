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
    -  12 subprecesos
    -  Hyper-Threading
  - 24 GB RAM
  - SSD 500 GB

---

## 🌐 Arquitectura de Red

- Router del ISP en modo bridge
- Host Proxmox
- VM OPNsense (firewall y routing)
- Switch gestionable (TP-Link SG608E)
- Punto de acceso WiFi (Huawei AX3)

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

---

## 🏠 Automatización Domótica

- Comunicación basada en MQTT
- Dispositivos ESP8266, ESP32 y NodeMCU
- Flujos Node-RED para automatización

---

## 🎯 Objetivos

- Evolucionar hacia prácticas DevOps
- Automatizar despliegues y tareas
- Mejorar monitorización y observabilidad

---

## 🚀 Mejoras futuras

- Integración de Docker
- Pipelines CI/CD
- Infraestructura como código (Ansible / Terraform)
- Monitorización avanzada (Prometheus + Grafana)
