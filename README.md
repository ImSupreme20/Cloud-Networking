# Google Cloud – Network Load Balancer (NLB) Lab

This repository documents my hands-on work completing the **Set Up Network Load Balancers** lab on Google Cloud. The lab walks through configuring a Layer 4 passthrough Network Load Balancer using Compute Engine virtual machines, firewall rules, health checks, and forwarding rules.

---

## 🚀 Lab Objectives

In this lab, I practiced how to:

- Configure default region and zone settings  
- Deploy multiple Compute Engine VM instances  
- Install and configure Apache web servers  
- Create firewall rules for HTTP traffic  
- Configure a Network Load Balancer (NLB)  
- Create a target pool and forwarding rule  
- Send traffic to the load balancer and observe distribution  

---

## 🧰 Technologies Used

- Google Cloud Platform (GCP)  
- Compute Engine  
- Cloud Shell  
- Network Load Balancer (L4 Passthrough)  
- gcloud CLI  

---

## 📌 Key Concepts Reinforced

| Concept | Summary |
|--------|---------|
| **L4 Load Balancing** | Routes traffic based on IP/port without inspecting packets |
| **Target Pools** | Group of backend instances for passthrough NLBs |
| **Forwarding Rules** | Define how traffic reaches backend services |
| **Health Checks** | Ensure only healthy instances receive traffic |
| **Firewall Rules** | Control inbound/outbound network access |

---

