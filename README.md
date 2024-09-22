# Describe Azure compute and Networking Services 

This module introduces Azure's compute and networking services. It covers Azure virtual machines, containers, Azure Functions, and networking features like Azure Virtual Networks, DNS, and ExpressRoute.

## Learning Objectives
- Compare compute types (virtual machines, container instances, and functions).
- Describe virtual machine options, including VM scale sets, availability sets, and Azure Virtual Desktop.
- Understand the resources required for virtual machines.
- Explore application hosting options: Azure Web Apps, containers, and VMs.
- Learn about virtual networking, including Azure Virtual Networks, subnets, peering, Azure DNS, VPN Gateway, and ExpressRoute.
- Define public and private endpoints.

---

## 1. Azure Virtual Machines (VMs)

Azure VMs provide **Infrastructure as a Service (IaaS)**, offering full control over the OS and application configuration. VMs are ideal for scenarios where you need:
- Total control over the OS.
- The ability to run custom software.
- Custom hosting configurations.

### Key VM Features
- **Preconfigured VM images:** Use templates that include OS and software to rapidly provision VMs.
- **Scale VMs:** You can run single VMs or group VMs for high availability and scalability using features like scale sets and availability sets.

### **Virtual Machine Scale Sets**
- **Scale sets** automate the management and scaling of a group of identical VMs.
- Azure handles load balancing, updates, and scaling based on demand.

### **Virtual Machine Availability Sets**
- Availability sets ensure VMs are grouped across **update domains** and **fault domains** to prevent downtime due to hardware or network failures.

---

## 2. Azure Virtual Desktop (AVD)
- **Azure Virtual Desktop (AVD)** is a cloud-hosted desktop and application virtualization service that allows access to Windows desktops from anywhere and on any device.
- **Key benefits:**
  - Centralized management and security.
  - Multi-session Windows 10 support.
  - Runs apps in proximity to the data center, improving performance.

---

## 3. Azure Functions

**Azure Functions** is a serverless, event-driven compute service. It allows you to run code triggered by events without managing the underlying infrastructure.

### Benefits of Azure Functions:
- **No infrastructure management:** Focus on code, not the server.
- **Auto-scaling:** Functions scale based on demand automatically.
- **Pay-as-you-go:** You're only billed for the compute resources your functions use.

### Use Cases:
- Real-time data processing.
- Lightweight APIs.
- Automating backend tasks.

---

## 4. Application Hosting Options in Azure

Azure offers multiple hosting solutions for applications:
- **Azure Virtual Machines:** Full control over the hosting environment.
- **Azure App Service:** Platform as a Service (PaaS) for web apps, APIs, and mobile apps. Offers automatic scaling and supports multiple programming languages.
- **Containers:** Lightweight, portable environments for running applications.

### Azure App Service Features:
- Supports Windows and Linux.
- Automatic scaling and high availability.
- Integration with CI/CD tools like GitHub and Azure DevOps.

---

## 5. Azure Virtual Networking

**Azure Virtual Networks** enable resources like VMs, web apps, and databases to communicate securely with each other and with on-premises environments.

### Networking Capabilities:
- **Isolation and segmentation:** Create isolated virtual networks with private IP address ranges.
- **Public and private endpoints:** Public endpoints allow internet access, while private endpoints are for internal communication.
- **Routing traffic:** Azure routes traffic between subnets, virtual networks, and the internet.

### Virtual Private Networks (VPNs):
- **Point-to-site:** Connects a single device to an Azure virtual network.
- **Site-to-site:** Connects an on-premises network to an Azure virtual network.
- **ExpressRoute:** Private, high-speed, low-latency connections between on-premises networks and Azure.

---

## 6. Azure Containers

**Containers** are lightweight virtualization environments that allow multiple instances of applications to run on the same host machine without managing the underlying OS.

### Key Container Services:
- **Azure Container Instances (ACI):** Fast and simple way to run containers without managing VMs.
- **Azure Kubernetes Service (AKS):** A container orchestration service for managing large-scale container deployments.

### Docker:
- **Docker** is a platform for building, running, and sharing containers. It packages applications and their dependencies in isolated environments, ensuring consistent operation across different environments.

---

## 7. ExpressRoute

**Azure ExpressRoute** allows private connections between on-premises networks and Azure, bypassing the public internet for more reliable and secure communication.

### Features:
- **Global connectivity:** Connect your on-premises sites via ExpressRoute circuits.
- **Dynamic routing:** Uses BGP for dynamic route exchange between on-premises and Azure resources.
- **Built-in redundancy:** Ensures high availability by using redundant devices for all connections.

---

## 8. Azure DNS

**Azure DNS** provides domain name resolution using Microsoft Azure’s infrastructure, enabling you to manage your DNS records alongside other Azure services.

### Key Benefits:
- **Global DNS network:** Provides high availability and fast performance through Azure's global network of DNS servers.
- **Security:** Integrated with Azure Resource Manager, offering Azure role-based access control (RBAC) and resource locking.
- **Private Domains:** Use custom domain names in private virtual networks.

---

## Key Questions

### 1. Which Azure Virtual Machine feature staggers updates across VMs based on their update domain and fault domain?
- **Answer:** Availability sets

### 2. Which Azure service allows users to use a cloud-hosted version of Windows from any location and connect from most modern browsers?
- **Answer:** Azure Virtual Desktop

### 3. Which type of VPN gateway should you use for connections between virtual networks, point-to-site, multisite connections, or coexistence with Azure ExpressRoute?
- **Answer:** Route-based VPN gateway

---

## Summary

In this module, you learned about Azure compute and networking services. This includes:
- Virtual machines, scale sets, availability sets, and Azure Virtual Desktop.
- Networking features like Azure Virtual Networks, VPN gateways, and ExpressRoute.
- Hosting options like Azure App Service, containers, and serverless computing (Azure Functions).
- Key networking concepts like private and public endpoints, DNS, and VPNs.

---

## Additional Resources
- **[Host a Web Application with Azure App Service](https://learn.microsoft.com/en-us/learn/modules/host-a-web-app-with-azure-app-service/)**: Explore the process of hosting web applications in Azure.
- **[Introduction to Azure Network Foundation Services](https://learn.microsoft.com/en-us/learn/paths/intro-to-azure-network-foundation-services/)**: Learn more about Azure networking.

