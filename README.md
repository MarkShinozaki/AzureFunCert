# Describe Cloud Service types 

## Cloud Service Types: IaaS, PaaS, and SaaS

This module covers the different cloud service types and their use cases and benefits:

- **Infrastructure as a Service (IaaS)**
- **Platform as a Service (PaaS)**
- **Software as a Service (SaaS)**
- **Appropriate Use Cases for Each Service Type**

---

## 1. Describe Infrastructure as a Service (IaaS)

**Infrastructure as a Service (IaaS)** is the most flexible category of cloud services, offering maximum control over cloud resources. In the IaaS model:

- **Cloud Provider's Responsibility:** 
  - Maintains hardware, network connectivity (to the internet), and physical security.
  
- **Customer's Responsibility:** 
  - Responsible for everything else, including:
    - Operating system installation, configuration, and maintenance.
    - Network configuration.
    - Database and storage configuration.

Essentially, you are renting the hardware in a cloud data center, and you manage the software layer and infrastructure.

### Shared Responsibility Model for IaaS
- IaaS places most of the responsibility on the customer.
- **Cloud provider** maintains the physical infrastructure and access to the internet.
- **Customer** is responsible for:
  - Installation and configuration.
  - Patching and updates.
  - Security.

### IaaS Scenarios

- **Lift-and-shift migration:**  
  Move your on-prem datacenter resources to the IaaS cloud infrastructure, approximating the on-prem environment in the cloud.

- **Testing & development:**  
  Quickly replicate development and test environments by starting and shutting down environments in an IaaS structure while maintaining full control.

---

## 2. Describe Platform as a Service (PaaS)

**Platform as a Service (PaaS)** is a middle ground between IaaS and SaaS, providing a complete development environment without the need to manage infrastructure.

- **Cloud Provider's Responsibility:**
  - Maintains physical infrastructure, security, internet connectivity, operating systems, databases, and development tools.

- **Customer's Responsibility:**
  - Focuses on application development without worrying about infrastructure maintenance, licensing, or patching.

### Shared Responsibility Model for PaaS
- **Cloud provider** maintains physical infrastructure, operating systems, and development tools.
- **Customer** may still manage networking settings, application security, and directory infrastructure, depending on the configuration.

### PaaS Scenarios

- **Development Framework:**  
  PaaS provides a framework for developing or customizing cloud-based applications. Features like scalability, high-availability, and multi-tenancy are included, reducing the need for developers to manage those aspects manually.

- **Analytics or Business Intelligence:**  
  PaaS includes tools that allow organizations to analyze and mine data, find patterns, predict outcomes, and improve business decisions.

---

## 3. Describe Software as a Service (SaaS)

**Software as a Service (SaaS)** provides fully developed software solutions delivered over the internet. Users interact directly with the application without worrying about managing the underlying infrastructure.

- **Cloud Provider's Responsibility:**
  - Handles everything, including infrastructure, operating systems, and the application itself.

- **Customer's Responsibility:**
  - Simply uses the software for its intended purpose.

### SaaS Scenarios

- **Business Applications:**  
  SaaS is well-suited for applications like email, CRM, ERP, and financial software, where the customer just needs to access the software without managing underlying systems.

---

## 4. Key Use Cases for IaaS, PaaS, and SaaS

- **IaaS:** Best for lift-and-shift migrations, testing, and development environments, or scenarios where full control over infrastructure is necessary.
- **PaaS:** Ideal for application development environments where developers need to focus on coding without managing infrastructure.
- **SaaS:** Best for accessing fully developed software applications like finance, CRM, and productivity tools without managing any underlying infrastructure.

---

## Shared Responsibility Model Overview

| Responsibility            | On-Premises    | IaaS          | PaaS          | SaaS          |
|---------------------------|----------------|---------------|---------------|---------------|
| **Physical Datacenter**    | Customer       | Cloud Provider| Cloud Provider| Cloud Provider|
| **Physical Network**       | Customer       | Cloud Provider| Cloud Provider| Cloud Provider|
| **Operating System**       | Customer       | Customer      | Cloud Provider| Cloud Provider|
| **Applications**           | Customer       | Customer      | Customer      | Cloud Provider|
| **Data & Information**     | Customer       | Customer      | Customer      | Customer      |

---

## Knowledge Check 

#### 1. Which cloud service type is most suited to a lift and shift migration from an on-prem datacenter to a cloud deployment? 
- [x] IaaS
- [ ] PaaS
- [ ] SaaS

  - With an IaaS service type, you can approximate your on-premises environment, making a lift-and-shift transition to the cloud relatively straightforward
     
#### 2. What type of cloud service type would be Finance and Expensive Tracking solution typically be in? 
- [ ] IaaS
- [ ] PaaS
- [x] SaaS

-  SaaS provides access to software solutions, such as finance and expense tracking, email or ticketing systems
