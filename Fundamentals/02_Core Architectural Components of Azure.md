# Core Architectural Components of Azure

## 1. Introduction
Microsoft Azure is a cloud computing platform that provides services for compute, networking, storage, and databases. It runs on a global infrastructure designed for high availability, scalability, and security.

---

## 2. Key Components of Azure Architecture

### 2.1 Azure Regions
- **Definition**: Geographical areas that contain one or more datacenters.
- **Purpose**: Enable customers to deploy services close to users for lower latency and compliance.
- **Types**:
  - **Region Pair**:
    - Two regions within the same geography.
    - Example: East US and West US.
    - Provide disaster recovery, failover, and update rollouts.
  - **Sovereign Regions**:
    - Dedicated to meet compliance and regulatory requirements.
    - Examples:
      - Azure Government (US Government usage).
      - Azure China (operated by 21Vianet).

---

### 2.2 Availability Zones
- **Definition**: Physically separate datacenters within a single Azure region.
- **Purpose**: High availability, fault tolerance, and redundancy.
- **Features**:
  - Independent power, cooling, and networking.
  - Protects applications and data from datacenter-level failures.
- **Usage Example**:
  - Deploying a multi-zone Virtual Machine (VM) setup for failover.

---

### 2.3 Azure Datacenters
- **Physical Layer of Azure**.
- **Security Measures**:
  - Multi-layered physical security.
  - Video surveillance, perimeter fencing, and biometric access.
- **Networking**:
  - Global low-latency, high-speed fiber optic backbone.
- **Redundancy**:
  - Power and cooling systems with backup generators.

---

## 3. Azure Management Infrastructure

### 3.1 Azure Resources
- **Definition**: Individual services such as Virtual Machines (VMs), databases, or storage accounts.
- **Management Tools**:
  - Azure Portal.
  - Azure PowerShell.
  - Azure CLI.
  - REST APIs.

---

### 3.2 Resource Groups
- **Definition**: Logical containers for organizing resources.
- **Purpose**:
  - Manage resources as a group.
  - Apply common policies, role-based access control (RBAC), and automation.
- **Lifecycle Management**:
  - Deleting a resource group deletes all associated resources.

---

### 3.3 Subscriptions
- **Purpose**: Define boundaries for billing, quotas, and access control.
- **Key Points**:
  - Each subscription is linked to an Azure account.
  - Multiple subscriptions can exist under one account for different departments, projects, or environments.

---

### 3.4 Management Groups
- **Definition**: Containers for managing multiple subscriptions.
- **Usage**:
  - Apply governance policies, RBAC, and compliance rules across multiple subscriptions.
- **Hierarchy**:
  - Management Group → Subscription → Resource Group → Resource.

---

## 4. Azure Hierarchy Overview
- **Purpose**: Ensures structured organization and streamlined access management.

---

## 5. Hands-On Exercises
1. **Explore Azure Portal and CLI**.
2. **Create a Resource Group**.
3. **Deploy a Resource (e.g., Virtual Machine)**.
4. **Apply a policy via Management Groups**.

---

## 6. Key Assessment Questions
1. What are Azure Regions, Region Pairs, and Sovereign Regions?
2. Difference between Resource Groups and Subscriptions?
3. Role of Management Groups in Azure governance?
4. What is the hierarchy of Azure resource management?

---

## 7. Summary
- Azure runs on a **global network of datacenters**, organized into regions and availability zones.
- **Resources** are grouped logically into **Resource Groups**, billed under **Subscriptions**, and managed via **Management Groups**.
- The layered hierarchy allows for **scalability, cost management, and secure access control**.

---
