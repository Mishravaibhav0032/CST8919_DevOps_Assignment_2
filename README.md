# Cloud Service Alternatives Report  
**Course:** CST8919 – DevOps Security and Compliance  
**Assignment:** 2 – Cloud Service Alternatives Report  
**Due Date:** 15th August, 2025  
**Author:** Vaibhav Mishra (041165850) 

---

## 📌 Objective
This report identifies equivalent services in **Amazon Web Services (AWS)** and **Google Cloud Platform (GCP)** for key **Microsoft Azure** services studied in the course.  
Each section includes an **overview**, **core features**, **security & compliance details**, **pricing model**, and **integration for DevSecOps**.  
A **comparison table** is provided for quick reference, followed by a narrative analysis.

The Azure services covered include:
- **Microsoft Entra ID** (for SSO and IAM)
- **Azure Monitor & Log Analytics**
- **Azure Policy**
- **Microsoft Defender for Cloud**
- **Microsoft Sentinel** (for SIEM/SOAR)

For each Azure service, equivalents in **Amazon Web Services (AWS)** and **Google Cloud Platform (GCP)** are identified. Comparisons are provided in terms of overview, core features, security & compliance, pricing model, and integration for DevSecOps.

---

## Comparison Table

| Azure Service                  | AWS Equivalent                               | GCP Equivalent                                           | Key Feature Differences                                                                                                   | Pricing Highlights                                                                                  |
|--------------------------------|-----------------------------------------------|----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Microsoft Entra ID             | AWS IAM Identity Center                       | Cloud Identity                                           | Azure emphasizes hybrid identity; AWS focuses on multi-account SSO; GCP integrates with Google Workspace                 | Azure: Tiered (Free, P1, P2); AWS: Free; GCP: Free/Premium editions                                |
| Azure Monitor & Log Analytics  | Amazon CloudWatch                             | Google Cloud Operations Suite (Monitoring & Logging)     | Azure integrates deeply with Log Analytics queries; AWS excels in alarms; GCP offers tiered data ingestion               | All pay-as-you-go based on data volume; free tiers available                                       |
| Azure Policy                   | AWS Organizations (with SCPs)                 | Organization Policy Service                              | Azure uses JSON policies for compliance; AWS for multi-account governance; GCP for hierarchical constraints               | All generally free                                                                                  |
| Microsoft Defender for Cloud   | AWS Security Hub                              | Security Command Center                                  | Azure supports multicloud CNAPP; AWS focuses on findings aggregation; GCP emphasizes AI protection                       | Azure: Free foundational + paid plans; AWS: Pay per checks/findings; GCP: Tiered (Standard free)   |
| Microsoft Sentinel             | Amazon Security Lake                          | Chronicle Security Operations                            | Azure is full SIEM/SOAR; AWS centralizes data lakes; GCP uses AI-driven analytics                                         | All pay-as-you-go on ingestion/storage; free trials                                                |

---

## Detailed Comparisons

### 1. Microsoft Entra ID (SSO, IAM)

**Equivalents:**
- AWS: AWS IAM Identity Center
- GCP: Cloud Identity

**Overview:**
- **Azure:** Cloud-based IAM enabling access to external/internal resources with support for admins, developers, and subscribers.
- **AWS:** Manages workforce access to AWS applications with centralized visibility.
- **GCP:** Unified identity, access, and endpoint management platform integrated with Google Workspace.

**Core Features:**
- **Azure:** MFA, conditional access, identity governance, hybrid identity, privileged identity management.
- **AWS:** Single sign-on, centralized access management, secure EC2 instance access.
- **GCP:** SSO, MFA, endpoint management.

**Security & Compliance:**
- **Azure:** MFA, risk-based conditional access, encryption, compliance tools.
- **AWS:** MFA, access auditing, compliance via policies.
- **GCP:** MFA, recognized in Forrester Wave for IaaS security.

**Pricing Model:**
- Azure: Free tier, P1 ($6/user/month), P2 ($9/user/month)
- AWS: Free
- GCP: Free edition, Premium $7.2/user/month

**Integration for DevSecOps:**
- **Azure:** API-based automation, CI/CD SSO integration.
- **AWS:** CLI/SDK integration, centralized monitoring.
- **GCP:** Limited automation details.

**Narrative Analysis:**
Azure leads with hybrid capabilities, AWS is best for multi-account setups, GCP excels in Workspace integration.

---

### 2. Azure Monitor & Log Analytics

**Equivalents:**
- AWS: Amazon CloudWatch
- GCP: Google Cloud Operations Suite

**Overview:**
- **Azure:** End-to-end monitoring, log querying via Log Analytics.
- **AWS:** Multi-source monitoring with alarms and integrations.
- **GCP:** Performance and health monitoring across environments.

**Core Features:**
- **Azure:** VM/container insights, dashboards, alerts, autoscale, AIOps.
- **AWS:** Alarm-based automation, dashboards, integration with 70+ AWS services.
- **GCP:** Tiered data ingestion, synthetic monitoring.

**Security & Compliance:**
- Azure: Integration with Defender and Sentinel.
- AWS: Compliance through alarms and policies.
- GCP: Supports audit logging.

**Pricing Model:**
- Azure: $2.30/GB ingestion (first 5GB/month free)
- AWS: ~$0.50/GB ingestion (5GB/month free)
- GCP: $0.258/MiB (free allotments)

**Integration for DevSecOps:**
- **Azure:** CI/CD integration via DevOps/GitHub.
- **AWS:** Automated alarms in pipelines.
- **GCP:** API-driven monitoring integration.

**Narrative Analysis:**
Azure excels in detailed querying, AWS in reactive alerting, GCP in cost-effective large-scale monitoring.

---

### 3. Azure Policy

**Equivalents:**
- AWS: AWS Organizations (SCPs)
- GCP: Organization Policy Service

**Overview:**
- **Azure:** JSON-defined policies with compliance tracking.
- **AWS:** Multi-account governance via service control policies.
- **GCP:** Constraints-based centralized resource control.

**Core Features:**
- **Azure:** Compliance dashboard, remediation, policy initiatives.
- **AWS:** Centralized policy application.
- **GCP:** Constraint inheritance, dry-run mode.

**Security & Compliance:**
- Azure: Built-in compliance mappings.
- AWS: CIS/PCI-aligned policy enforcement.
- GCP: Constraint enforcement and auditing.

**Pricing Model:**
- Azure: Free (Azure), $6/server/month (Arc)
- AWS: Free
- GCP: Free

**Integration for DevSecOps:**
- **Azure:** Policy-as-code integration.
- **AWS:** Touchless multi-account enforcement.
- **GCP:** YAML/JSON pipeline testing.

**Narrative Analysis:**
Azure’s remediation features align with DevSecOps automation goals.

---

### 4. Microsoft Defender for Cloud

**Equivalents:**
- AWS: AWS Security Hub
- GCP: Security Command Center

**Overview:**
- **Azure:** Multicloud CNAPP with lifecycle security.
- **AWS:** Findings aggregation for prioritization.
- **GCP:** AI and risk-focused security operations.

**Core Features:**
- **Azure:** Secure score, attack path analysis, DevOps security.
- **AWS:** Unified visibility, automated checks.
- **GCP:** Vulnerability scanning, compliance workflows.

**Security & Compliance:**
- Azure: Threat hunting, compliance monitoring.
- AWS: CIS/PCI mapping.
- GCP: Compliance library.

**Pricing Model:**
- Azure: Free foundational, CSPM $15/server/month
- AWS: Pay per checks/findings
- GCP: Tiered pricing

**Integration for DevSecOps:**
- Azure: GitHub/Azure DevOps pipeline integration.
- AWS: Ticketing system integration.
- GCP: Limited detail.

**Narrative Analysis:**
Azure’s multicloud coverage fits advanced compliance needs.

---

### 5. Microsoft Sentinel

**Equivalents:**
- AWS: Amazon Security Lake
- GCP: Chronicle Security Operations

**Overview:**
- **Azure:** SIEM/SOAR with advanced automation.
- **AWS:** Centralized security data lake.
- **GCP:** AI-driven detection and response.

**Core Features:**
- **Azure:** Data connectors, threat hunting, playbooks.
- **AWS:** Data normalization and analysis.
- **GCP:** Threat detection and analytics.

**Security & Compliance:**
- Azure: Tamper-proof logs.
- AWS: Customer-owned data controls.
- GCP: Compliance monitoring.

**Pricing Model:**
- Azure: $2.25/GB ingestion
- AWS: ~$0.75/GB ingestion
- GCP: Usage-based

**Integration for DevSecOps:**
- Azure: Playbooks with Logic Apps.
- AWS: Centralized ingestion for analysis.
- GCP: Supports automation.

**Narrative Analysis:**
Sentinel fits course log analysis needs; AWS and GCP offer alternatives suited for data aggregation and AI-enhanced detection.

## References
- Microsoft Azure Documentation  - https://learn.microsoft.com/en-us/azure/?product=popular  
- AWS Documentation   
- Google Cloud Documentation  
