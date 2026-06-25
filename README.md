# Azure Compute & Deployment Models — Hands-on Exploration

## Overview
This repository documents a structured, hands-on exploration of Azure compute services and deployment mechanisms completed as part of the AZ-900T00-A course.  
The focus is on understanding architectural intent, operational trade-offs, and automation strategies across IaaS and PaaS models.

---

## Labs Completed
- Create a Virtual Machine in the Portal
- Create a Web App
- Deploy Azure Container Instances
- Implement Azure Functions
- Create a VM with an ARM Template
- Create a VM with PowerShell
- Create a VM with Azure CLI

---

### Azure CLI Resource Management in Cloud Shell

#### Overview
Expanded hands-on experience with Azure CLI by using Cloud Shell to create, manage, query, and clean up Azure resources directly from the command line. This lab reinforces automation‑ready workflows and demonstrates how CLI-based operations streamline deployment and lifecycle management.

#### Objectives
- Navigate and operate within Azure Cloud Shell  
- Create and manage resources using Azure CLI commands  
- Apply tags, query resources, and perform cleanup from the command line  

#### Tasks Performed

##### 1. Explore Cloud Shell Environment
- Launched Cloud Shell in Bash mode, verified subscription context, explored built‑in help, and listed available regions.

**Outcome:**  
Cloud Shell environment initialized with full command-line readiness.

##### 2. Create and List Resources with CLI
- Created a resource group and two storage accounts entirely through CLI commands.
- Listed and filtered resources to validate successful deployment.

**Outcome:**  
A resource group and two storage accounts created and verified using CLI commands.

##### 3. Tag, Query, and Clean Up Resources
- Applied tags to the resource group and individual resources.
- Used JMESPath filters to query and shape CLI output.
- Deleted the resource group to complete the full lifecycle from the command line.

**Outcome:**  
Resources tagged, queried, and cleaned up entirely through Azure CLI operations.

---

### Enable High Availability with Availability Sets

#### Overview
Implemented high availability for virtual machines by distributing workloads across an Azure availability set and fronting them with a load balancer. This lab demonstrates how Azure protects applications from hardware failures and ensures resilient compute architectures.

#### Objectives
- Create and configure an availability set  
- Deploy multiple virtual machines across fault and update domains  
- Add and configure an Azure Load Balancer  
- Implement health probes and load‑balancing rules  

#### Tasks Performed
- Created an availability set to distribute VM workloads across isolated hardware.  
- Deployed two virtual machines into the availability set.  
- Added an Azure Load Balancer to provide a unified entry point for the VMs.  
- Configured a health probe to monitor VM availability.  
- Added a load‑balancing rule to distribute traffic across both VMs.

**Outcome:**  
A highly available VM architecture using an availability set and load balancer, providing resilience against hardware failures and enabling balanced traffic distribution.

---

## Compute Models Compared

| Model               | Control Level | Operational Overhead  | Best Use Case                              |
|---------------------|---------------|-----------------------|--------------------------------------------|
| Virtual Machine     | Full          | High                  | Legacy systems, full OS control            |
| App Service         | Limited       | Low                   | Web apps with minimal infrastructure needs |
| Container Instances | Medium        | Low                   | Lightweight, isolated workloads            |
| Azure Functions     | Minimal       | Very Low              | Event-driven logic, reactive tasks         |

---

## Deployment Methods Explored

| Method      | Type           | Benefits                            |
|-------------|----------------|-------------------------------------|
| Portal      | Manual         | Quick for testing, not scalable     |
| ARM Template| Declarative IaC| Repeatable, version-controlled      |
| PowerShell  | Scripted       | Automation-friendly, Windows-native |
| CLI         | Scripted       | Cross-platform, DevOps-ready        |

---

## Key Learnings
- Azure offers layered compute abstractions to balance control vs. simplicity.
- Infrastructure-as-Code (IaC) enables repeatable, auditable deployments.
- Serverless models reduce operational burden but require architectural discipline.
- Deployment method choice affects scalability, governance, and automation potential.

---

## Next Steps
- Explore networking and security integration across compute models.
- Transition to operational scenarios in AZ-104 and AZ-305.
- Apply IaC principles to multi-resource environments.


