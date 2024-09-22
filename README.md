# Describe the Core Architectural Components of Azure 

Microsoft Azure is a continually expanding set of cloud services that help you meet current and future business challenges. Azure gives you the freedom to build, manage, and deploy applications on a massive global network using your favorite tools and frameworks.

---

## Azure Accounts, Subscriptions, Resource Groups, and Resources

### **Azure Free Account:**
- Free access to popular Azure products for 12 months.
- A credit to use for the first 30 days.
- Access to over 25 products that are always free.

### **Azure Free Student Account:**
- Free access to certain Azure services for 12 months.
- A credit to use for the first 12 months.
- Free access to certain software developer tools.

---

## Azure Physical Infrastructure

Azure's core architecture is divided into **physical infrastructure** and **management infrastructure**.

### **1. Physical Infrastructure:**
- **Datacenters:** Facilities containing racks of resources with dedicated power, cooling, and networking.
- **Regions:** A geographical area containing at least one datacenter, connected via low-latency networks. Resources are balanced across these regions.
- **Availability Zones:** Physically separate datacenters within a region, each with independent power, cooling, and networking. They provide an **isolation boundary** in case one zone goes down.
  - Three or more availability zones are required in a zone-enabled region.
  
### **2. Region Pairs:**
- Azure pairs regions within the same geography to provide additional resilience.
  - If a region in a pair is affected by a disaster, services fail over to the paired region.
  - Example: West US is paired with East US.
  
### **3. Sovereign Regions:**
- Isolated instances of Azure designed for compliance and legal purposes.
  - Examples: **US DoD Central**, **US Gov Virginia**, **China East** (in partnership with 21Vianet).

---

## Azure Management Infrastructure

### **Azure Resources and Resource Groups:**
- **Resources:** The basic building block in Azure (e.g., VMs, databases, networks).
- **Resource Groups:** Logical groupings of resources that allow for easy management.
  - A resource can only be in one resource group at a time, and resource groups cannot be nested.

### **Azure Subscriptions:**
- **Subscriptions** allow you to manage, bill, and scale your resources.
  - **Billing Boundary:** Each subscription is billed separately.
  - **Access Control Boundary:** Azure applies access-management policies at the subscription level.
  
- You can create additional subscriptions to manage different environments, billing, or organizational structures.

### **Azure Management Groups:**
- Provide an extra level of hierarchy above subscriptions, allowing for better access, policies, and compliance management.
  - Management groups can be nested and all settings are inherited by the subscriptions and resources under them.

---

## Azure Resources for Resiliency

### **Availability Zones:**
- Ensure redundancy by hosting mission-critical applications across multiple zones.
  - **Zonal Services:** Pin resources to a specific zone (e.g., VMs, managed disks).
  - **Zone-Redundant Services:** Automatically replicated across zones (e.g., SQL databases).
  - **Non-Regional Services:** Resilient to zone-wide and region-wide outages.

### **Region Pairs:**
- Pairs regions within the same geography for disaster recovery and compliance.
  - Azure ensures that one region in each pair is prioritized for recovery during a large-scale outage.
  - Example: **West US** is paired with **East US**.

---

## Key Azure Terms and Concepts

- **Datacenter:** The physical infrastructure that holds computing resources in racks, equipped with power, cooling, and networking.
- **Region:** A geographical area that houses datacenters connected via a low-latency network.
- **Availability Zone:** A physically separate data center within a region to improve resiliency.
- **Region Pair:** Two Azure regions within the same geography for disaster recovery and backup.
- **Resource:** Any Azure service (VMs, storage, databases, etc.) created or provisioned by users.
- **Resource Group:** A container for resources, helping manage them collectively.
- **Subscription:** A logical grouping that allows for resource management, billing, and access control.
- **Management Group:** A level of hierarchy above subscriptions for organizing and governing large-scale environments.

---

## Important Considerations

- **Redundancy and Resiliency:** Using availability zones and region pairs improves the reliability of applications.
- **Management Efficiency:** Azure subscriptions and management groups help organizations efficiently manage billing and access for large, complex environments.
- **Sovereign Regions:** For specific compliance needs, sovereign regions offer isolated instances of Azure.

--- 

## Knowledge Check



### 1. How many resource groups can a resource be in at the same time?
- [x] One
- [ ] Two
- [ ] Three
  - **A resource can only be in one group at a time.**

### 2. What happens to the resources within a resource group when an action or setting is applied to the resource group?
- [ ] Current resources inherit the setting, but future resources don’t.
- [ ] Future resources inherit the settings, but current ones don’t.
- [x] **The setting is applied to current and future resources.**


