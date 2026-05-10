
# Homelab Infrastructure & Portfolio Site

This repository contains the Infrastructure-as-Code (IaC) used to deploy and manage my professional portfolio and lab documentation site. Features include a containerized documentation stack and MkDocs-Material deployment on Docker/Proxmox with UniFi-backed VLAN segmentation.

## 🛠️ Technology Stack
- **Hypervisor:** Proxmox VE
- **Runtime:** Docker / Docker Compose
- **Documentation Engine:** MkDocs Material
- **Reverse Proxy:** Nginx Proxy Manager (NPM)
- **Edge Security:** Cloudflare (SSL/DNS)

## 🌐 Network Architecture
The site is hosted on a containerized stack within my home lab, utilizing a **UniFi Ultra** ecosystem.
- **VLAN Segmentation:** Production traffic is isolated from the development sandbox.
- **Persistence:** Volume mapping is used to ensure data integrity during container updates.

## 📂 Deployment
To deploy this stack locally:
1. Ensure Docker and Docker Compose are installed.
2. Clone this repository.
3. Run `docker-compose up -d`.
