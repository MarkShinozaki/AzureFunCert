# Describe Cloud Computing 


### Learning Objectives 
- Define Cloud Computing
- Describe the Shared Responsibility Model
- Define Cloud Models, including public, private and hybrid
- Identify appropriate use cases for each cloud model
- Describe the consumption-based model
- Compare cloud models


### What is Cloud Computing 
- Cloud Computing is the delivery of computing services over the internet. Computing services include common IT infrastructure such as virtual machines, storage, databases and networking. Cloud services also expand the traditional IT offerings to include things like IoT, ML and AI.

- Since Cloud computing uses the internet to deliver these services, it doesnt have to be constrained by physical infrastructure the same way that a traditional datacenter is.

- That means if you need to increase your IT infrastructure rapidly, you dont have to wait to build a new datacenter, you can use the cloud to rapidly expand your IT footprint.

- The two services provided by most cloud providers are compute power and storage.

--- 

### Describe the Shared Responsibility Model 

- WIth a traditional corporate datacenter. The company is responsible for maintaining the physical space, ensuring security, and maintaining for replacing the servers if anything happens. The IT department is responsible for maintaining all the infrastructure and software needed to keep the datacenter up and running 

- The Shared responsibility Model means these responsibilities get shared between the cloud provider and the consumer. Physical security, power, cooling, and network connectivity are responsibility of the cloud provider.


> [!IMPORTANT]
> If you deploy a virtual machine and installed an SQL database on it, the consumer is responsible for database patches and updates
> WIth an on-premises datacenter, the consumer is responsible for everything



| Responsibility                   | On-prem | IaaS        | PaaS        | SaaS        |
|----------------------------------|---------|-------------|-------------|-------------|
| **Information and data**         | Customer| Customer    | Customer    | Customer    |
| **Devices (Mobile and PCs)**     | Customer| Customer    | Customer    | Customer    |
| **Accounts and identities**      | Customer| Customer    | Customer    | Shared      |
| **Identity and directory infrastructure** | Customer| Shared      | Shared      | Cloud Provider |
| **Applications**                 | Customer| Customer    | Shared      | Cloud Provider |
| **Network controls**             | Customer| Customer      | Shared      | Cloud Provider |
| **Operating system**             | Customer| Customer      | Cloud Provider | Cloud Provider |
| **Physical hosts**               | Customer| Cloud Provider | Cloud Provider | Cloud Provider |
| **Physical network**             | Customer| Cloud Provider | Cloud Provider | Cloud Provider |
| **Physical datacenter**          | Customer| Cloud Provider | Cloud Provider | Cloud Provider |


#### WHen using a cloud provider, you'll always be responsible for:
- The information and data stored in the cloud
- Devices that are allowed to connect to your cloud (cell phones, computers, and so on)
- The accounts and identifies of the people, services, and devices within your organization

#### The cloud provider is always responsible for:
- The physical datacenter
- The physical network
- The physical hosts

#### your services model will determine responsibility for things like:
- Operating Systems
- Network Controls
- Applications
- Identity Infrastructure 

---

### Cloud Models
- Cloud models define the type of cloud environment based on how resources are deployed. The three primary cloud models are:

#### Private Cloud:

- Definition: A cloud environment dedicated to a single entity (organization). It offers greater control over resources and security, as the organization manages the infrastructure.

- Advantages:
  - Complete control over resources and security.
  - Data isn't shared with other organizations.

- Challenges:
  - Higher cost due to hardware purchases and maintenance.
  - Fewer benefits like scalability compared to public cloud.

- Hosting Options: It can be hosted on-premises or in an offsite dedicated datacenter, possibly managed by a third party.

#### Public Cloud:

- Definition: A cloud environment built, managed, and maintained by a third-party provider (e.g., Microsoft Azure, AWS, Google Cloud). Resources are available to anyone who wishes to purchase and use them.

- Advantages:
  - No capital expenditures to scale up.
  - Organizations pay only for what they use (pay-as-you-go).
  - Applications can be quickly provisioned and deprovisioned.

- Challenges:
  - Less control over resources and security, as they are managed by the cloud provider.

#### Hybrid Cloud:

- Definition: Combines both public and private clouds in an interconnected environment. This model allows organizations to use private cloud infrastructure while taking advantage of the public cloud for additional resources when needed.

- Advantages:
  - Provides flexibility to scale between private and public clouds based on demand.
  - Control over where applications and data reside.
  - Offers an extra layer of security by determining which services remain in private infrastructure.

- Challenges:
  - Requires managing two cloud environments, which can add complexity.

#### Multi-Cloud:

- Definition: Involves using multiple public cloud providers (e.g., AWS and Azure). Organizations might choose different providers based on the specific features they offer or to avoid vendor lock-in.

- Advantages:
  - Flexibility in using the best services from multiple providers.
  - Ability to spread risk across different cloud environments.

- Challenges:
  - Requires managing resources, security, and costs across multiple cloud platforms.

### Key Concepts

#### Azure Arc:

- Definition: A set of technologies from Microsoft Azure that helps organizations manage their cloud environments, whether they are using Azure public cloud, private cloud, hybrid cloud, or even multi-cloud setups involving multiple cloud providers.

- Use Cases: Azure Arc simplifies managing resources, governance, security, and compliance across different cloud environments from a single control plane.

#### Azure VMware Solution:

- Definition: A service that allows organizations already using VMware in a private cloud environment to seamlessly migrate their VMware workloads to Azure. This enables scalability and integration with Azure services without requiring modifications to VMware tools or processes.

- Use Case: Perfect for organizations wanting to move from private cloud to public or hybrid cloud setups without disrupting existing VMware-based workflows.

| **Public Cloud**                               | **Private Cloud**                            | **Hybrid Cloud**                             | **Multi-Cloud**                              |
|------------------------------------------------|----------------------------------------------|---------------------------------------------|---------------------------------------------|
| No capital expenditures to scale up.           | **Organizations control all resources.**        | Flexibility to scale between environments.  | **Multiple public cloud providers used.**       |
| Quick provisioning/deprovisioning.             | **Dedicated resources (no sharing).**            | Decide which services stay public/private.  | **Access features from different providers.**   |
| Pay for what you use (pay-as-you-go).          | **Must purchase hardware and maintain it.**      | Improved security by separating data.       | **Avoids vendor lock-in, spreading risk.**      |
| Less control over resources/security.          | **High setup and maintenance costs.**            | Best for temporary demand surges.           | **Must manage multiple environments.**         |

--- 

## Describe the consumption based Model 

### CapEx (Capital Expenditures) vs. OpEx (Operational Expenditures) in IT infrastructure 

- #### Capital Expenditure (CapEx):
  - A one-time, upfront investment in physical resources like buildings, data centers, vehicles or equipment
  - Examples: Building a new data center, purchasing servers, or buying company vehicles.
  - CapEx involves owning and managing the infrastructure yourself
 
- #### Operatonal Expenditure (OpEx):
  - Ongoing costs for services or products, paid for over time.
  - Examples: Renting space, leasing vehicles, or subscribing to cloud services
  - Cloud computing falls under OpEx because you're paying for what you use without owning the physical infrastructure. 


### Consumption-Based Model in Cloud Computing 
- #### What it is:
  - A pricing model where you only pay for the cloud resources you actually use, like virtual machines, storage, or network badnwidth
 
- #### Key Benefits:
  - No upfront costs: you dont need to buy expensive infrastructure in advance
  - Flexibility: You can scale resources up or down as needed
  - Pay-as-you-go: Only pay for what you use. When resources are no longer needed, you stop paying for them
  - No wasted resources: Avoid over-provisioning, which can lead to wasted costs, or under-provisioning, which can cause performance issues.

- #### Why it's beneficial:
  - Traditional data centers require accurate predictions of future resource needs, which can lead to over or under-provisioning. In contrast, cloud computing allows dynamic scaling where you can easily add or remove resources, avoiding the risks associated with incorrect capacity planning. 

### Cloud pricing Models 

- Cloud computing operates on pay-as-you-go pricing models, meaning you only pay for what you use. This has several benefits for managing costs: 
  - Plan and manage costs: CLoud models enable better control over operating expenses since you're not investing large sums of money upfront like in a CapEx model.
  - Run more efficiently: Since you can easily scale resources as demand fluctuates, you can run your infrastructure more efficiently without needing to over-provision or guess future demand
  - Scalability: As your business needs change, cloud services can scale up or down, enabling you to align your infrastructure with real-time demands
 
### Key Differences between CLoud and Traditional Datacenters
- #### Traditional Datacenter:
  - Requires upfront investment (CapEx) for infrastructure and hardware
  - You must plan future resource needs in advance, which may lead to either over-provisioning (wasted resources) or under-provisioing (performance issues).
  - Scaling up takes time, as you need to purchase, install, and configure new hardware
 
- #### Cloud-Based Model:
  - Operates on a consumption-based model (OpEx) where you only pay for what you use.
  - Resources are scalable on-demand (e.g., virtual machines), and you can add or remove them as needed without downtime or significant planning
  - Cloud providers handle the maintenance and infrastructure, allowing business to focus on applications and services. 

--- 

## Check Knowledge 

### 1. What is cloud computing?
- [x] **Delivery of computing Services over the internet**
- [ ] Delivery of storage services over the internet
- [ ] Delivery of websites via the internet

  - #### Cloud computing is the delivery of computing services over the internet 

### 2. Which cloud model uses some datacenters focused on providing cloud services to anyone that wants them, and some data centers that are focused on a single customer?
- [ ] Public Cloud
- [x] **Hybrid Cloud**
- [ ] Multi-cloud

  - #### THe Hybrid cloud model is a combination of public cloud and private cloud, using both datacenters dedicated solely to one customer and datacenter that are shared with the public
     
### 3. According to the shared responsibility model, which cloud service type places the most resonsibility on the customer? 
- #### IaaS places the most responsibility on the customer, with the cloud provider being responsible for the basics of physical security, power and connectivity

--- 

## Additional Resources 

- #### [Shared responsibility model](https://learn.microsoft.com/en-us/azure/security/fundamentals/shared-responsibility) - is the sharing of responsibilities for the cloud between you and your cloud provider

- #### [Introduction to Azure Vmware Solution](https://learn.microsoft.com/en-us/learn/modules/intro-azure-vmware-solution/)- is a Microsoft Learn course that dives deeper into Azure VMware Solution 

- #### More about [Hybrid Cloud](https://learn.microsoft.com/en-us/learn/modules/intro-to-azure-hybrid-services/)


