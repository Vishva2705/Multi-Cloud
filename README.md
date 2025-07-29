# 🚀 Multi-Cloud Application with AWS and Azure

This project explores a production-grade **multi-cloud architecture**, leveraging both **Amazon Web Services (AWS)** and **Microsoft Azure** to ensure high availability, resilience, and scalability. The solution implements **intra-cloud** and **inter-cloud load balancing**, aiming to mitigate the risk of provider-level outages and infrastructure failures.

Designed with distributed cloud principles in mind, this architecture allows for seamless failover, load distribution, and state consistency across providers.

---

## 🧱 Architecture Overview

![Multi-Cloud Architecture](https://github.com/NAchref/Multi-Cloud-Application-with-Load-Balancing-on-AWS-and-Azure/blob/main/PLAN%20%26%20ARCHITECTURE/Architecture.jpg)

- **Frontend & API:** Containerized Django application
- **Databases:** AWS RDS (MySQL) and Azure SQL
- **Compute:** AWS EC2, Azure Virtual Machines
- **Load Balancing:**
  - **AWS Elastic Load Balancer (ELB)**
  - **Azure Load Balancer**
- **High Availability:** Active-active deployment across clouds

---

## 🎯 Objectives

- Architect and deploy a **fault-tolerant multi-cloud application**
- Ensure **zero downtime** during cloud-specific failures
- Implement **dynamic load balancing** at both intra-cloud and inter-cloud levels
- Maintain **data consistency and state replication** across cloud providers
- Leverage **Docker containers** for platform-agnostic deployment

---

## 🗓️ Development Plan

### Sprint 1: Local Environment Setup
- Develop a modular Django e-commerce application with full CRUD operations
- Implement service-level abstraction to support future portability

### Sprint 2: Cloud Service Integration
- Deploy backend on Azure App Services and connect to Azure SQL
- Deploy backend on AWS EC2 and connect to AWS RDS (MySQL)
- Validate performance, latency, and endpoint consistency

### Sprint 3: Containerization & CI/CD Pipeline
- Dockerize Django app for consistent cloud deployment
- Configure container orchestration on both platforms
- Push containers to EC2 (AWS) and Azure VM

### Sprint 4: Load Balancing & Resiliency Testing
- Deploy **AWS Elastic Load Balancer** for intra-cloud distribution
- Deploy **Azure Load Balancer** for mirrored configuration
- Simulate node and cloud failure scenarios
- Measure failover response, latency, and recovery time

---

## ⚙️ Technologies & Tools

| Category          | Technology                     |
|------------------|---------------------------------|
| Cloud Platforms  | AWS, Microsoft Azure            |
| Application      | Django (Python)                 |
| Databases        | AWS RDS (MySQL), Azure SQL      |
| Deployment       | Docker, Azure VM, AWS EC2       |
| Load Balancing   | AWS ELB, Azure Load Balancer    |
| CI/CD            | GitHub Actions (Optional)       |
| Monitoring (optional) | CloudWatch, Azure Monitor     |

---

## 📈 Outcome

- Achieved **multi-cloud deployment** with distributed database connectivity
- Maintained **service availability during simulated cloud outages**
- Successfully demonstrated **cross-cloud load balancing and failover**
- Reduced cloud vendor lock-in risk with a flexible deployment strategy

---

## 📌 Future Improvements

- Implement cross-cloud session persistence
- Integrate DNS-level load balancing (e.g., AWS Route 53 + Azure Traffic Manager)
- Add monitoring dashboards and SLA tracking
- Extend architecture to support Kubernetes or multi-region deployment

---

## 📄 License

This project was developed for educational and research purposes as part of the **CODTECH Internship – Task 3: Multi-Cloud Architecture**. All components can be reused or extended under appropriate attribution.

