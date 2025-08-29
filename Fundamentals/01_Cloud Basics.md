# Azure Fundamentals (AZ-900) Notes

---

## 1. What is Cloud Computing?

Basically, it's renting IT stuff instead of buying it.
- **On-demand:** Get what you need, when you need it.
- **Over the internet:** Access it from anywhere.
- **Pay-as-you-go:** Like an electricity bill; only pay for what you use.

### The Big Idea: CapEx vs. OpEx
| | CapEx (Capital Expenditure) | OpEx (Operational Expenditure) |
| :--- | :--- | :--- |
| **What it is** | Buying stuff upfront. | Paying for a service as you use it. |
| **Analogy** | Buying a car. | Leasing a car or using Uber. |
| **IT Example** | Buying servers for your basement. | Renting a virtual server from Azure. |
| **Model** | Old-school, on-premises. | Modern, cloud. |

---

## 2. Cloud Deployment Models

How you can set up your cloud:

1.  **Public Cloud:**
    - The most common type. Run by huge companies (Microsoft, Amazon, Google).
    - **Pros:** Cheap, no maintenance, super scalable.
    - **Cons:** You share the hardware with others (but your data is still private).

2.  **Private Cloud:**
    - Your own personal cloud. You own or rent the hardware just for you.
    - **Pros:** More control, more security.
    - **Cons:** Expensive, you handle maintenance.

3.  **Hybrid Cloud:**
    - A mix of public and private. They are connected.
    - **Use Case:** Keep secret data in your private cloud but run your public website on the public cloud.

---

## 3. The Shared Responsibility Model

**This is super important.** Security is a shared job between you and the cloud provider.

| | **Provider's Responsibility** | **Your Responsibility** |
| :--- | :--- | :--- |
| **On-Premises** | Nothing. You do everything. | The physical server, OS, apps, data, access |
| **IaaS** (Virtual Machines) | Physical security, network, storage | OS, apps, data, access |
| **PaaS** (App Services, Databases) | OS, runtime, network, storage | Your data and application access |
| **SaaS** (Office 365) | Everything except... | Your data and user access |

**Simple Rule:** The cloud provider **always** handles the physical stuff. You **always** handle your data and access.

---

## 4. The Consumption-Based Model

- The core pricing model of the cloud.
- **No upfront costs.** You don't sign a contract for a year.
- You are billed **precisely** for what you consume (e.g., per hour for a VM, per GB for storage).
- This makes costs **predictable** and avoids wasting money on idle resources.

---

## 5. Why Use the Cloud? (Key Benefits)

- **High Availability:** Your stuff stays online, even if one part fails. (e.g., 99.9% uptime)
- **Scalability:** Handling more users by adding more resources.
    - **Vertical Scaling (Scale Up):** Make your single server bigger (add CPU/RAM).
    - **Horizontal Scaling (Scale Out):** Add more servers to share the load (better way!).
- **Elasticity:** This is automatic scaling. It can scale out during busy times and scale in during quiet times to save money.
- **Reliability:** The system can fix itself and keep running if something breaks.
- **Security:** Cloud providers have massive security teams and tools built-in (firewalls, encryption).
- **Manageability:** You can automate tasks and manage everything through a web portal or scripts.

### TCO (Total Cost of Ownership)
- A tool to compare the total cost of running your workload on-premises vs. in the cloud.
- It includes hidden costs like power, cooling, and IT admin time.
- Almost always shows that the cloud is cheaper.

---
### Module 1 Checklist:
- [ ] Understand CapEx vs. OpEx
- [ ] Know the difference between Public, Private, Hybrid cloud
- [ ] Memorize the Shared Responsibility Model
- [ ] Get why the consumption model is useful
- [ ] Know the key benefits (Elasticity, Scalability, etc.)
