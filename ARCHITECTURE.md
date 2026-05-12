# Architecture Details
<img width="1263" height="752" alt="Capture d’écran 2026-05-05 002254" src="https://github.com/user-attachments/assets/54e55fc5-2476-456c-bf9f-7ec40a150413" />

This document explains the internal architecture of the lab.

## Components
- DVWA → Target application
- MySQL → Database
- phpMyAdmin → DB interface
- Kali → Attacker machine
- Monitoring stack → cAdvisor → Prometheus → Grafana

## Network
All services run inside the "cyber_lab" Docker network.

## Data Flow
Kali → DVWA → MySQL  
cAdvisor → Prometheus → Grafana
