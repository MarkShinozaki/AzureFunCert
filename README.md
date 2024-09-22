# Describe Azure Management and Governance 

## Introduction

In this module, you'll be introduced to the factors that impact costs in Azure and tools that help you predict, monitor, and control costs.

### Learning Objectives

- Describe factors that can affect costs in Azure.
- Compare the pricing calculator and Total Cost of Ownership (TCO) calculator.
- Describe the Microsoft Cost Management Tool.
- Describe the purpose of tags.

---

## Factors that Affect Costs in Azure

Azure shifts costs from **CapEx** (capital expense) to **OpEx** (operational expense), offering flexibility and scalability. Various factors influence OpEx:

### Key Factors:
- **Resource Type**: The type and settings of the resources provisioned will impact the cost.
- **Consumption**: Pay-as-you-go pricing or reserved capacity for discounts.
- **Maintenance**: Managing resources, ensuring unused resources are deprovisioned to avoid excess costs.
- **Geography**: Prices vary by region due to factors like power, labor, and taxes.
- **Network Traffic**: Inbound data transfers are generally free; outbound data is priced based on zones.
- **Subscription Type**: Some subscriptions, like free trials, come with usage allowances.
- **Azure Marketplace**: Solutions from third-party vendors can affect costs.

---


## Comparing Pricing and TCO Calculators

### Pricing Calculator

- Estimates the cost of provisioning resources in Azure.
- Focuses on individual or grouped resources and configurations.
- Prices shown are estimates, and no actual resources are provisioned.

### TCO Calculator

- Helps compare the cost of running an on-premises infrastructure versus an Azure cloud infrastructure.
- Takes into account factors like power, IT labor costs, and storage requirements to provide a cost comparison.

---

## Exercise - Estimate Workload Costs with the Pricing Calculator

Steps to estimate the cost of running a basic web application using the **Azure Pricing Calculator**:

1. Define the services needed (e.g., Virtual Machines, SQL Database, and Application Gateway).
2. Configure the services (region, operating system, instance type, etc.).
3. Use the calculator to generate an estimated cost.
4. Export, save, or share the estimate for collaboration.

---


## Exercise - Compare Workload Costs using the TCO Calculator

The **TCO Calculator** is used to compare the costs of running a sample workload on-premises versus in Azure. It involves three steps:

1. **Define your workloads**: Enter specifications of the current on-premises infrastructure.
2. **Adjust assumptions**: Modify cost factors like currency and region.
3. **View the report**: Generate and review the report for cost savings over a set timeframe (e.g., three years).

---



## Microsoft Cost Management Tool

**Cost Management** helps you manage and control Azure spending by providing insights and setting budgets. It includes:

### Key Features:
- **Cost Analysis**: Visualize and explore costs by billing cycle, region, or resource type.
- **Cost Alerts**: Set alerts for budgets, credit limits, and departmental spending quotas.
- **Budgets**: Set spending limits on subscriptions or resource groups and receive alerts when limits are reached.
- **Automation**: Advanced budgets can trigger automated responses, like suspending resources when a budget is exceeded.

---



## Tags

Tags are used to organize Azure resources by providing additional metadata for resource management.

### Use Cases:
- **Resource Management**: Tags help locate and manage resources related to specific workloads or departments.
- **Cost Management**: Group resources by tags to report on costs and track budgets.
- **Operations**: Group resources by their availability and importance to business operations.
- **Security**: Classify data based on security level, such as public or confidential.
- **Governance and Compliance**: Ensure resources align with regulatory requirements.
- **Workload Optimization**: Visualize all resources in complex deployments for automation or management.

### Example Tagging Structure:
| Name       | Value                |
|------------|----------------------|
| AppName    | The name of the application |
| CostCenter | Internal cost center code   |
| Owner      | Responsible business unit   |
| Environment| Prod, Dev, or Test          |
| Impact     | Mission-critical, High, Low |

---



## Knowledge Check

1. **What Azure feature helps stay organized by tracking resource metadata?**
   - **Answer**: Tags
2. **What’s the best method to estimate migration costs to the cloud?**
   - **Answer**: Use the Total Cost of Ownership (TCO) calculator to estimate expected costs.

---



## Summary

In this module, you learned about factors that impact costs in Azure and the tools that help you predict, monitor, and control costs.

### Learning Objectives:

- Describe factors that can affect costs in Azure.
- Compare the Pricing Calculator and Total Cost of Ownership (TCO) calculator.
- Describe the Microsoft Cost Management Tool.
- Describe the purpose of tags.

---

# Additional Resources

- **Control Azure spending and manage bills with Microsoft Cost Management + Billing** - This learning path provides a deeper understanding of cost management tools and strategies in Azure.

[Learn More](https://learn.microsoft.com/en-us/learn/paths/control-spending-manage-bills/)

