# CST8912 Lab 7

**Student Name**: Collin MacLeod
**Student ID**: macl0379
**Course**: CST8912 Cloud Solutions Architecture
**Semester**: Fall 2026

---

## Introduction

Cloud provider provides a variety of cloud services in a variety of cloud service models: IaaS, PaaS, and SaaS. When businesses migrate to the cloud, they must choose which model is best suited to their needs and is the most cost-effective. This course is designed to assist Cloud Architects in identifying their current cloud expenditures and providing greater awareness of the costs associated with each deployment model as well as each aspect of a cloud deployment.

Optimizing cloud costs begins with knowing your current cloud expenditures. This course introduces you to the tools built into the cloud Portal that can help you understand the total overall expenditures in cloud as well as break down those costs by area: Compute, Network, Storage, Identity, and App/Cloud Services.

The remainder of the course drills down on specific costs associated with each area of cloud identifies the costs associated with each service and provides very clear and concise methods for reducing cloud expenditures. Many of the cost savings methods will require minimal changes to your cloud deployment and will take just minutes to implement while other cost savings methods may take a shift in your cloud strategy, such as moving from Iaas to PaaS. 

---

## Screenshots

### Step 1 - Template Deployment

![Custom Deployment Template](/Screenshots/Custom%20Deploy%20Template.png "Custom Deployment Template")
*Figure 1.1: Custom deployment template*


![Custom Deployment Parameters page with values](/Screenshots/Custom%20Deployment%20Parameters.png "Custom Deployment Parameters page with values")
*Figure 1.2: Custom deployment parameters page with values*


![Custom Deployment in Progress](/Screenshots/Custom%20Deployment%20in%20Progress.png "Custom Deployment in Progress")
*Figure 1.3: Custom deployment in progress*


![Custom Deployment Review Page](/Screenshots/Custom%20Deployment%20Review%20Page.png "Custom Deployment Review Page")
*Figure 1.4: Custom deployment review page*


### Step 2 - Create Alert Rule


![Alert Rule Scope](/Screenshots/Alert%20Rule%20Scope.png "Alert Rule Scope")
*Figure 2.1: Alert rule scope*


![Alert Rule Condition](/Screenshots/Alert%20Rule%20Condition.png "Alert Rule Condition")
*Figure 2.2: Alert rule condition*


### Step 3 - Configure Action Group Notifications


![Action Group Basics](/Screenshots/Action%20Group%20Basics.png "Action Group Basics")
*Figure 3.1: Action group basics*


![Action Group Notifications](/Screenshots/Action%20Group%20Notifications.png "Action Group Notifications")
*Figure 3.2: Action group notifications*


![Subscribed to Notifications](/Screenshots/Subscribing%20to%20Alerts.png "Subscribed to Notifications")
*Figure 3.3: Subscribed to notifications*


### Step 4 - Trigger Alert


![Delete VM](/Screenshots/Delete%20VM.png "Delete VM")
*Figure 4.1: Delete VM*


![Alert Details](/Screenshots/Alert%20Detail%20Screen.png "Alert Details")
*Figure 4.2: Alert details*


![Alert Email](/Screenshots/Azure%20Alert%20Email.png "Alert Email")
*Figure 4.3: Alert email*


### Step 5 - Configure Alert Proccessing Rule


![Alert Proccessing Rule Details](/Screenshots/Alert%20Proccessing%20Rule%20Details.png "Alert Proccessing Rule Details")
*Figure 5.1: Alert proccessing rule details*


![Alert Proccessing Rule Scheduling](/Screenshots/Alert%20Proccessing%20Rule%20Scheduling.png "Alert Proccessing Rule Scheduling")
*Figure 5.2: Alert proccessing rule scheduling*


![Alert Proccessing Rule Review](/Screenshots/Alert%20Proccessing%20Rule%20Validation.png "Alert Proccessing Rule Review")
*Figure 5.3: Alert proccessing rule review*


### Step 6 - Azure Monitor Log Queries


![Heartbeat Count Query](/Screenshots/Heartbeat%20Count%20Query.png "Heartbeat Count Query")
*Figure 6.1: Heartbeat Count Query*


![Insight Metrics Query](/Screenshots/Insight%20metrics%20query.png "Insight Metrics Query")
*Figure 6.2: Insight Metrics Query*


### Issues

In this lab I ran into 2 issues:

- When using the template to deploy the resources, I would receive alerts about vm quotas having a current limit of 0 (figure 7.1). To resolve this I used an azure CLI command to determine sizes that were similar in nature to the reccommended sizes that were available to me (figure 7.2).
- The alert was created three times and fired multiple emails and logged multiple times (figure 7.3). This would be an issue as it could clog logs and create possible confusion.


![VM Quota Error](/Screenshots/Verification%20Failed.png "VM Quota Error")
*Figure 7.1: VM quota error*

![Azure CLI command and output](/Screenshots/List%20of%20SKUs%20available%20in%20region.png "Azure CLI command and output")
*Figure 7.2: Azure CLI command and output*


---


## Cleanup

![Resource Group Cleanup](/Screenshots/Cleanup.png "Resource Group Cleanup")
*Figure 8: Resource group cleanup*

