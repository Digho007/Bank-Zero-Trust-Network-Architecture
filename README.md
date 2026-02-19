# Bank Zero Trust Network Architecture  
## Defense-in-Depth Security Blueprint for a Multinational Financial Institution

**Author:** Jeremiah Dighomanor  
**Domain:** Network Security Architecture / Cyber Defense  
**Project Type:** Enterprise Security Design (Capstone)  
**Program:** Developers Foundry Fellowship 2.0 (Tech4Dev)

---

## Executive Overview

Financial institutions are among the most targeted organizations globally.  
This project designs a **production-grade Zero Trust network architecture** for a multinational bank, focused on protecting critical assets, reducing attack surface, and ensuring operational resilience.

The architecture applies:

- Zero Trust principles  
- Defense-in-Depth strategy  
- Network segmentation  
- Least privilege enforcement  
- Continuous monitoring  

This repository demonstrates the ability to design secure infrastructure at enterprise scale.

---

## Business Problem

Banks must simultaneously:

- Provide highly available online services
- Protect sensitive financial data
- Detect threats rapidly
- Comply with strict regulations
- Prevent lateral movement after breaches

Traditional flat networks cannot meet these requirements.

---

## Solution Overview

A segmented, multi-zone architecture that isolates systems by trust level and function.

### Security Zones

| Zone | Purpose |
|------|--------|
DMZ | Public-facing services
Application Tier | Business logic processing
Data Tier | Sensitive databases and storage
Corporate Network | Employee systems
Management Network | Administrative control plane
Guest/Partner Network | External access isolation

Critical policy:

> No direct communication from Internet or DMZ to the Data Tier.

---

## Architecture Highlights

### External Protection

- DDoS mitigation
- Next-Generation Firewall (HA)
- Intrusion Prevention System
- Web Application Firewall

### Internal Protection

- Network segmentation
- Database firewall
- Network Access Control
- Endpoint Detection & Response
- Data Loss Prevention

### Identity & Access

- Multi-factor authentication
- Privileged Access Management
- Jump server for administrative access

### Monitoring & Detection

- Centralized SIEM
- Log aggregation and correlation
- Threat detection workflows

---

## Traffic Security Model

Example — Online Banking Transaction:

Internet  
→ DDoS Protection  
→ Perimeter Firewall  
→ IPS  
→ WAF  
→ Load Balancer  
→ Web Servers (DMZ)  
→ Application Tier  
→ Data Tier  

All flows are inspected, authenticated, and logged.

---

## Implementation Strategy

Phased deployment to avoid business disruption:

1. Perimeter defense and segmentation
2. Advanced detection and application security
3. Endpoint and privileged controls
4. Continuous improvement

---

## Security Outcomes

- Reduced attack surface
- Contained breach impact
- Faster detection and response
- High service availability
- Strong regulatory alignment

---

## Metrics Targets

- MTTD < 15 minutes
- MTTR < 1 hour
- 99.99% uptime
- 95% patch compliance

---

## Repository Contents

- `/diagram` — Network and traffic flow diagrams
- `/assets/exports` — Original project deliverables

---

## Skills Demonstrated

- Enterprise network architecture design
- Security control placement
- Threat modeling
- Zero Trust implementation
- Incident detection strategy
- Defense-in-Depth planning

---

## Author

**Jeremiah Dighomanor**  
Cybersecurity Engineer | Security Architect

---

## License

MIT
