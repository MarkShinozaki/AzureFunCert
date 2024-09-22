# Describe Monitoring tools in Azure 


## Introduction

This module introduces tools for monitoring both Azure and on-premises or multicloud environments.

### Learning Objectives:
- Understand the purpose of Azure Advisor.
- Learn about Service Health.
- Explore Azure Monitor, including Azure Log Analytics, Azure Monitor Alerts, and Application Insights.

---

## Azure Advisor

Azure Advisor analyzes Azure resources to provide recommendations that help improve reliability, security, performance, operational excellence, and cost-efficiency. It is accessible via the Azure portal and API.

### Features:
- Personalized recommendations.
- Notifications for new recommendations.
- Recommendations categorized into:
  - Reliability
  - Security
  - Performance
  - Operational Excellence
  - Cost

---

## Azure Service Health

Azure Service Health offers detailed information about the health of Azure services that you use as well as global Azure services.

### Components:
- **Azure Status**: Provides a global view of the health of Azure services.
- **Service Health**: Offers personalized alerts and views of the health of the Azure services and regions you are using.
- **Resource Health**: Gives detailed health information about your specific resources.

---

## Azure Monitor

Azure Monitor is a comprehensive solution for collecting, analyzing, and acting on telemetry from your cloud and on-premises environments.

### Key Components:
- **Azure Log Analytics**: Tool for writing and running log queries using data gathered by Azure Monitor.
- **Azure Monitor Alerts**: Automates notifications and actions based on metrics and log data.
- **Application Insights**: Monitors the performance and usage of live applications.

### How it works:
- Collects data from all layers of your application architecture.
- Stores data in central repositories.
- Analyzes data using queries, visualizations, and alerts.

---

## Knowledge Check

1. **Which is not one of the recommendation categories for Azure Advisor?**
   - The correct answer is "Capacity". The categories are Reliability, Security, Performance, Operational Excellence, and Cost.

2. **If you receive a notification of an Azure region outage, which Azure Service Health component would inform you if your resources are impacted?**
   - **Resource Health** provides detailed health information about your individual Azure resources.

---

## Summary

You should now be able to describe key Azure tools for monitoring and managing resources effectively, ensuring optimal performance, security, and cost management in Azure and beyond.

### Additional Resources
- [Get Started with Azure Advisor](https://learn.microsoft.com/en-us/learn/modules/get-started-azure-advisor/)
- [Intro to Azure Service Health](https://learn.microsoft.com/en-us/learn/modules/intro-to-azure-service-health/)
- [Azure Monitor Learning Path](https://learn.microsoft.com/en-us/learn/paths/monitor-usage-performance-availability-resources-azure-monitor/)

