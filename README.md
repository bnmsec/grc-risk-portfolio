# GRC Risk Portfolio

Commercial risk assessment and POA&M remediation tracking aligned to NIST CSF 2.0 and HIPAA Security Rule.

## Artifacts

- [Risk Assessment Package (PDF)](Risk_Assessment_Package_Commercial_v1.2.pdf) - Full assessment with executive summary, control statements, implementation evidence, threat model, and POA&M tracker
- [POA&M Tracking Register (XLSX)](POAM_Tracking_Register.xlsx) - Standalone remediation tracker with risk ratings, SLAs, and status tracking
- [Third-Party Risk Assessment Framework (PDF)](Third_Party_Risk_Assessment_Framework_v1.1.pdf) - Internal TPRM methodology with criticality tiers, four-domain evaluation, and scoring matrix
- [Vendor Security Questionnaire (XLSX)](Vendor_Security_Questionnaire_v1.1.xlsx) - External intake form for Medium/High criticality vendors with instructions, 16-question assessment, and internal scoring reference

## Framework Alignment

- NIST Cybersecurity Framework 2.0
- HIPAA Security Rule (164.308, 164.312)
- NIST SP 800-53 Rev 5 (source controls)

## Design Rationale

### Why These Five Controls
I selected AC-3, SC-7, AU-2, SI-4, and IA-2 because they represent the highest-impact controls for a cloud-based logistics platform handling PII and PHI. I excluded controls like CP-9 (backup) and PE-3 (physical access) because they are inherited from AWS infrastructure and would inflate the assessment scope without reflecting the team's direct responsibility. Scoping discipline matters. An over-scoped assessment creates noise. An under-scoped one creates gaps.

### Why NIST CSF 2.0 and HIPAA Instead of CMMC
This assessment was originally built against NIST 800-53 and CMMC Level 2. I translated it to NIST CSF 2.0 and HIPAA because those are the frameworks healthcare organizations and commercial MSPs actually audit against. The crosswalk on Page 2 of the PDF demonstrates framework fluency. I can read one framework and speak another. NIST 800-53 remains the master control catalog underneath both frameworks. The crosswalk demonstrates that I can select rigorous technical controls and translate them into business and regulatory language for different audiences.

### Why Logistics-Specific Vendor Categories
The Third-Party Risk Assessment names ELD providers, fuel card services, factoring companies, and freight brokers because those are the actual vendor categories in transportation. Generic TPRM templates list generic SaaS providers. I listed the vendors I spent 12 years managing. Specificity signals operational experience.

### Why This POA&M Structure
The POA&M tracker includes resource allocation because remediation without budget context isn't realistic. Every entry has a dollar sign behind it, even if that dollar sign is "we need to request budget."

### What I Would Do Differently
With more time and access, I would expand the assessment to 12-15 controls covering backup, incident response, and physical security. I would add quantitative risk scoring instead of qualitative High/Medium/Low. I would build a vendor registry with automated reassessment triggers. This portfolio represents a focused five-control assessment. A production engagement would be broader. I am aware of the difference.

## Contact

- Email: brandon@bnmsec.com
- LinkedIn: https://linkedin.com/in/brandon-schuerenberg
- Website: https://bnmsec.com
