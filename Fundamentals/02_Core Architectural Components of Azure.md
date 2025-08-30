# 🌐 Core Architectural Components of Azure

---

> **Level:** Beginner  
> **Role Targeted:** Administrator | Developer | DevOps | Architect  
> **Duration:** ~48 mins  
> **Exam Focus:** AZ-104, AZ-305  

---

## 🏙️ 1. Azure Regions

- **What are Azure Regions?**  
  Geographical areas that host Azure datacenters to ensure low latency, redundancy, and compliance.

### 📌 Key Points
- Each region has one or more datacenters.
- Regions are paired for disaster recovery.

| Type | Description | Example |
|------|-------------|---------|
| **Region Pair** | Two linked regions for failover & updates | East US & West US |
| **Sovereign Region** | Special compliance-based regions | Azure China, Azure Government |

---

## 🏢 2. Availability Zones
- Physically separate datacenters within a region.
- Independent power, cooling, and networking for **high availability**.

### 🎯 Benefits
- Fault tolerance at datacenter level.  
- Disaster recovery support.  

---

## 🏢 3. Azure Datacenters
- **Physical facilities** where Azure's hardware infrastructure resides.

### 🛡️ Security & Design
- Multi-layer security: Biometric access, CCTV, fencing.  
- Redundant power, cooling, and network systems.

---

## 🛠️ 4. Azure Management Infrastructure

### 4.1 Azure Resources
- **Definition:** Individual services (VMs, Databases, Storage Accounts).  
- **Managed via:** Azure Portal, CLI, PowerShell, REST APIs.

---

### 4.2 Resource Groups
- Logical containers for resources.  
- **Benefits:**  
  - Easy management (create, update, delete as a group).  
  - Policy & Role-Based Access Control (RBAC) application.  

---

### 4.3 Subscriptions
- Define billing, quotas, and access boundaries.  
- Multiple subscriptions can exist under a single Azure account.

---

### 4.4 Management Groups
- Containers for organizing multiple subscriptions.  
- Governance tool for applying policies & RBAC across multiple subscriptions.

---

## 📊 Azure Resource Hierarchy
```mermaid
graph TD
    MG[Management Group] --> SUB[Subscription]
    SUB --> RG[Resource Group]
    RG --> R[Resource]
