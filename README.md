# GRC Risk Portfolio

Cloud-native risk assessment and POA&M remediation tracking aligned to NIST CSF 2.0 and HIPAA Security Rule. Built against AWS infrastructure.

## Artifacts

- [Risk Assessment Package (PDF)](Risk_Assessment_Package_Commercial_v1.2.pdf) – Five-control assessment of an AWS-hosted logistics platform. Includes executive summary, NIST CSF 2.0 control statements, implementation evidence mapped to AWS services, threat model with three actor profiles, and integrated POA&M tracker.
- [POA&M Tracking Register (XLSX)](POAM_Tracking_Register.xlsx) – Standalone remediation tracker with risk ratings, resource allocation, SLAs, and status tracking.
- [Third-Party Risk Assessment Framework (PDF)](Third_Party_Risk_Assessment_Framework_v1.1.pdf) – Internal TPRM methodology with criticality tiers, four-domain evaluation, and scoring matrix.
- [Vendor Security Questionnaire (XLSX)](Vendor_Security_Questionnaire_v1.1.xlsx) – External intake form for Medium/High criticality vendors with instructions, 16-question assessment, and internal scoring reference.
- [Vendor Registry (XLSX)](Vendor_Registry_v1.0.xlsx) – Centralized vendor tracking with criticality tiers, assessment schedules, and open POA&M counts.

## Framework Alignment

- NIST Cybersecurity Framework 2.0
- HIPAA Security Rule (164.308, 164.312)
- NIST SP 800-53 Rev 5 (source controls)

**Methods:** NIST 800-53 control selection, NIST CSF 2.0 mapping, HIPAA Security Rule crosswalk, qualitative risk scoring, POA&M lifecycle tracking, vendor criticality tiering.

## Cloud Relevance

The controls assessed map directly to AWS services:

| Control | AWS Service |
|---------|-------------|
| AC-3 (Access Enforcement) | IAM policies and roles |
| SC-7 (Boundary Protection) | VPC security groups, API Gateway, subnet segmentation |
| AU-2 (Event Logging) | CloudTrail, CloudWatch |
| SI-4 (System Monitoring) | GuardDuty, Security Hub |
| IA-2 (Authentication) | IAM Identity Center, MFA enforcement |

The assessment was written against a cloud-based logistics platform running in AWS us-east-1, so the control mappings are cloud-native, not theoretical.

## Design Rationale

### Why These Five Controls

I selected AC-3, SC-7, AU-2, SI-4, and IA-2 because they represent the highest-impact controls for a cloud-based logistics platform handling PII and PHI. I excluded controls like CP-9 (backup) and PE-3 (physical access) because they are inherited from AWS infrastructure and would inflate the assessment scope without reflecting the team's direct responsibility. Scoping discipline matters. An over-scoped assessment creates noise. An under-scoped one creates gaps.

### Why NIST CSF 2.0 and HIPAA Instead of CMMC

This assessment was originally built against NIST 800-53 and CMMC Level 2. I translated it to NIST CSF 2.0 and HIPAA because those are the frameworks healthcare organizations and commercial MSPs actually audit against. The crosswalk on Page 2 of the PDF demonstrates framework fluency. I can read one framework and speak another. NIST 800-53 remains the master control catalog underneath both frameworks. The crosswalk demonstrates that I can select rigorous technical controls and translate them into business and regulatory language for different audiences.

### Why Logistics-Specific Vendor Categories

The Third-Party Risk Assessment names ELD providers, fuel card services, factoring companies, and freight brokers because those are the actual vendor categories in transportation. Generic TPRM templates list generic SaaS providers. I listed the vendors I spent 12 years managing. Specificity signals operational experience.

### Why This POA&M Structure

The POA&M tracker includes resource allocation because remediation without budget context isn't realistic. Every entry has a dollar sign behind it, even if that dollar sign is "we need to request budget."

## What This Portfolio Demonstrates

| Capability | Artifact |
|------------|----------|
| Vendor classification and risk tiering | TPRM Framework |
| Technical control assessment | Risk Assessment Package |
| Vendor evidence collection | Vendor Questionnaire |
| Remediation tracking with resource allocation | POA&M Register |
| Continuous monitoring and oversight | Vendor Registry |
| Framework translation (NIST ↔ HIPAA) | Risk Assessment Package (Crosswalk) |

## What I Would Do Differently

With more time and access, I would expand the assessment to 12–15 controls covering backup, incident response, and physical security. I would add quantitative risk scoring instead of qualitative High/Medium/Low. I would build a vendor registry with automated reassessment triggers. This portfolio represents a focused five-control assessment. A production engagement would be broader. I am aware of the difference.

## Contact

- Email: brandon@bnmsec.com
- LinkedIn: https://linkedin.com/in/brandon-schuerenberg
- Website: https://bnmsec.com
