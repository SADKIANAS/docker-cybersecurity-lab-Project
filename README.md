# 🚀 Docker-Based Cybersecurity Lab

## 📌 Overview
This project is a complete cybersecurity lab built using Docker Compose. It simulates a real-world environment for penetration testing, container management, and infrastructure monitoring.

---

## 🏗️ Architecture

<img width="1263" height="752" alt="Capture d’écran 2026-05-05 002254" src="https://github.com/user-attachments/assets/e54cd118-08a7-4212-bc4a-d3e8eba1cecd" />

<img width="487" height="221" alt="Capture d’écran 2026-05-01 220505" src="https://github.com/user-attachments/assets/0d4e0580-00d5-494a-8592-9e03d574f87c" />



The lab is composed of multiple layers:

- **Application Layer**: DVWA, phpMyAdmin  
- **Database Layer**: MySQL  
- **Pentesting Layer**: Kali Linux  
- **Monitoring Layer**: cAdvisor → Prometheus → Grafana  
- **Administration Layer**: Portainer  

All services are connected through an isolated Docker network.

---

## 🔧 Technologies Used

- Docker & Docker Compose  
- DVWA (Vulnerable Web App)  
- Kali Linux  
- MySQL & phpMyAdmin  
- Prometheus  
- Grafana  
- cAdvisor  
- Portainer  

---

## 📊 Monitoring System

 <img width="1058" height="907" alt="Capture d’écran 2026-04-25 170217" src="https://github.com/user-attachments/assets/69078ecf-cb09-4f73-b189-3054ea6962e9" />
 <img width="1267" height="481" alt="Capture d’écran 2026-04-25 160057" src="https://github.com/user-attachments/assets/633be9e7-35e8-4137-830a-7e8063633411" />
 <img width="1918" height="1021" alt="Capture d’écran 2026-04-24 181616" src="https://github.com/user-attachments/assets/64eae40e-0cb2-43f4-a9e9-9797b560a258" />
<img width="1897" height="887" alt="Capture d’écran 2026-04-24 181424" src="https://github.com/user-attachments/assets/96c0b6cc-9ecf-43e5-b639-1b8946e4530e" />
<img width="1132" height="827" alt="Capture d’écran 2026-04-24 181541" src="https://github.com/user-attachments/assets/97c15d9e-af19-4fff-9e6b-abad81d2a7a9" />
<img width="1410" height="637" alt="Capture d’écran 2026-04-24 181450" src="https://github.com/user-attachments/assets/7348eddd-1f94-4347-9dd3-3db75d8b622f" />
<img width="1918" height="922" alt="Capture d&#39;écran 2026-04-25 155757" src="https://github.com/user-attachments/assets/13f3020f-5e58-480a-baef-5bbad2083084" />



The monitoring pipeline works as follows:


- **cAdvisor** collects container metrics  
- **Prometheus** stores and processes metrics  
- **Grafana** visualizes data in dashboards  

---

## 🐳 Running Containers

<img width="1918" height="905" alt="Capture d&#39;écran 2026-04-23 103922" src="https://github.com/user-attachments/assets/7583ae2a-4cc4-4b88-a1ec-4111cbc696c8" />


All services are orchestrated using Docker Compose and run in isolated containers.

---

## 🗄️ Database Management (phpMyAdmin)

phpMyAdmin provides a web-based interface to manage the MySQL database used by DVWA.

It allows:
- Executing SQL queries  
- Managing tables and records  
- Inspecting stored data  

This simplifies database interaction during testing and analysis.

<img width="1901" height="907" alt="Capture d’écran 2026-04-23 104655" src="https://github.com/user-attachments/assets/196dd1a6-08d9-4afb-9b23-83030922fd83" />

## 🎯 Features

- Multi-container architecture  
- Isolated Docker network (cyber_lab)  
- Real-time monitoring  
- Persistent storage using volumes  
- Container management via Portainer  
- Simulated attack environment  


---

## ⚔️ Attack Simulation

This lab includes a simulated attack flow:


Used for practicing penetration testing in a safe and controlled environment.

---

<img width="1917" height="1017" alt="Capture d’écran 2026-04-11 171025" src="https://github.com/user-attachments/assets/147e5509-398e-4cb4-a2e7-43e4d8b57fa7" />
<img width="1067" height="218" alt="Capture d’écran 2026-04-25 181932" src="https://github.com/user-attachments/assets/edd2a99e-6053-4c0d-a698-b6820c1d79e1" />


## 🚀 How to Run

```bash
docker compose up -d


Access
DVWA → http://localhost:8080
phpMyAdmin → http://localhost:8081
Grafana → http://localhost:3000
Prometheus → http://localhost:9090
Portainer → http://localhost:8000
cAdvisor → http://localhost:8082

```

<img width="1562" height="838" alt="Capture d’écran 2026-04-25 165101" src="https://github.com/user-attachments/assets/73a3741b-ff45-4188-9667-20671c773cbc" />


📌 Notes

This project is intended for educational purposes only.
All testing must be performed in a controlled environment.
