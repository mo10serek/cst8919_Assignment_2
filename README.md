# Cloud Services Alternative Report

In the course, we learn a lot of different services in Azure cloud that uses for implementing security in our architecture. Now, I will explain the comparisons to the resources we use in Azure to resources to other cloud services such as AWS (Amazon Web Services) and GCP (Google Cloud Platform).

## Azure Active Directory (SSO, IAM)

| Azure Service | AWS | Google Cloud |
| Azure AD | AWS IAM Identity | Google Cloud Identity |

### Overview

-	**Azure AD**: It is a built in identify and access management service that use SSO, MFA, and role-based access control (RBAC)
-	**AWS IAM Identity**: An AWS’s solution for SSO and multi account management.
-	**Google Cloud Identity**: Google IAM service for managing users, groups, and policies

### Core Features
| Feature | Azure AD | AWS IAM Identity | Google Cloud Identity |
| SSO | have | have | have |
| MFA | have | have | have |
| RBAC | have | have | have |
| Directory Sync | Azure AD Connect | AWS Directory Service | Google Cloud Directory Sync |

### Security & Compliance

-	All support SOC 2, ISO 27001, GDPR
-	Azure AD: Deep integration with Microsoft 365.
-	Azure IAM: integrates with AWS Organizations
-	Google Cloud Identity: supports BeyondCorp Zero Trust.

### Pricing Model

-	Azure AD: Free tier and premium tier with $6 per month
-	AWS IAM Identity Center: Free
-	Google Cloud Identity: with $6 per month

### Integration with DevSecOps

-	All support CI/CD integration
-	Use Terraform and Ansible modules for automation

## Azure Monitor & Log Analytics

| Azure Service | AWS | Google Cloud |
| Azure Monitor | Amazon CloudWatch | Google Cloud Operations Suite |

### Overview

- **Azure Monitor**: Full-stack monitoring for apps, infrastructure, and networks.
- **CloudWatch**: AWS’s monitoring and observability service.
- **Google Cloud Operations**: GCP’s unified monitoring, logging, and diagnostics.

### Core Features

| Feature | Azure Monitor | CloudWatch | Google Cloud Operations |
| Log Analytics | have | CloudWatch Logs | Cloud Logging |
| Metrics & Alerts | have | have | have |
| Distributed Tracing | Application Insights | X-Ray | Cloud Trace |

### Security & Compliance

- All support encryption at rest and in transit.
- HIPAA, PCI DSS compliant.
### Pricing Model

- Azure Monitor: Pay-as-you-go (~$2.30/GB for logs).
- CloudWatch: Free tier; Log storage at $0.50/GB/month.
- Google Operations: Free tier; Logging at $0.50/GB/month.

### Integration for DevSecOps

- All integrate with Kubernetes, serverless, and CI/CD pipelines.
- Prometheus/Grafana support in all three.

## Azure Policy

| Azure Service | AWS Equivalent | Google Cloud |
| Azure Policy | AWS Config | Google Cloud Security Command Center (SCC) |

### Overview

- Azure Policy: Enforces compliance rules across Azure resources.
- AWS Config: Tracks resource configurations and compliance.
- GCP SCC: Security and risk management platform.

### Core Features

| Feature | Azure Policy | AWS Config | SCC |
| Compliance Checks | have | have | have | 
| Auto-Remediation | have | AWS System Manager | have | 
| Custom Policies | have | have | have |

### Security & Compliance

- All support CIS Benchmarks, NIST, HIPAA.

### Pricing Model

- Azure Policy: Free for basic policies.
- AWS Config: $0.003 per configuration item.
- GCP SCC: $0.0025/resource/hour.

### Integration for DevSecOps

- All support Terraform, CLI, and API automation.

## Microsoft Defender for Cloud

| Azure Service | AWS Equivalent | GCP Equivalent |
| Defender for Cloud | AWS Security Hub | Google Cloud Security Command Center (SCC) |

### Overview

- Defender for Cloud: Cloud security posture management (CSPM) and threat protection.
- AWS Security Hub: Centralized security alerts and compliance checks.
- GCP SCC: Unified security and threat detection.

### Core Features

| Feature | Defender for Cloud | AWS Security Hub | Google Cloud Security Command Center (SCC) |
| Vulnerability Scanning | have | have | have | 
| Threat Detection | have | have | have | 
| Compliance Dashboards | have | have | have |

### Pricing Model

- Defender for Cloud: Starts at $15/server/month.
- AWS Security Hub: $0.001 per finding.
- GCP SCC: $0.0025/resource/hour.

## Microsoft Sentinel (SIEM/SOAR)

| Service | AWS Equivalent | GCP Equivalent |
| Microsoft Sentinel | Amazon GuardDuty + AWS Detective | Google Chronicle |

### Overview

- Sentinel: Cloud-native SIEM with SOAR capabilities.
- GuardDuty: Threat detection service.
- Chronicle: Google’s security analytics platform.

### Pricing Model

- Sentinel: $4.50/GB log ingestion.
- GuardDuty: $1.00 per 1M events.
- Chronicle: Custom pricing.

## Summary table

| Feature | Azure AD | AWS IAM Identity | Google Cloud Identity |
| Azure AD | AWS IAM Identity | Google Cloud Identity |
| Azure Monitor | Amazon CloudWatch | Google Cloud Operations Suite |
| Azure Policy | AWS Config | Google Cloud Security Command Center (SCC) |
| Defender for Cloud | AWS Security Hub | Google Cloud Security Command Center (SCC) |
| Microsoft Sentinel | Amazon GuardDuty + AWS Detective | Google Chronicle |

