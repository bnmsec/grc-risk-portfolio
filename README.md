# GRC Risk Portfolio

Commercial risk assessment and POA&M remediation tracking aligned to NIST CSF 2.0 and HIPAA Security Rule.

## Artifacts

- [Risk Assessment Package (PDF)](Risk_Assessment_Package_Commercial_v1.2.pdf) - Full assessment with executive summary, control statements, implementation evidence, and POA&M tracker
- [POA&M Tracking Register (XLSX)](POAM_Tracking_Register.xlsx) - Standalone remediation tracker with risk ratings, SLAs, and status tracking

## Framework Alignment

- NIST Cybersecurity Framework 2.0
- HIPAA Security Rule (164.308, 164.312)
- NIST SP 800-53 Rev 5 (source controls)

## Design Rationale

### Why These Five Controls
I selected AC-3, SC-7, AU-2, SI-4, and IA-2 because they represent the highest-impact controls for a cloud-based logistics platform handling PII and PHI. I excluded controls like CP-9 (backup) and PE-3 (physical access) because they are inherited from AWS infrastructure and would inflate the assessment scope without reflecting the team's direct responsibility. Scoping discipline matters. An over-scoped assessment creates noise. An under-scoped one creates gaps.

### Why NIST CSF 2.0 and HIPAA Instead of CMMC
This assessment was originally built against NIST 800-53 and CMMC Level 2. I translated it to NIST CSF 2.0 and HIPAA because those are the frameworks Nashville healthcare organizations and commercial MSPs actually audit against. The crosswalk on Page 2 of the PDF demonstrates framework fluency. I can read one framework and speak another. That is the job.

### Why Logistics-Specific Vendor Categories
The Third-Party Risk Assessment names ELD providers, fuel card services, factoring companies, and freight brokers because those are the actual vendor categories in transportation. Generic TPRM templates list "SaaS providers." I listed the vendors I spent 12 years managing. Specificity signals operational experience.

### Why This POA&M Structure
The POA&M tracker includes resource allocation (Funded/Unfunded/Reallocation) because remediation without budget context is fiction. I have seen remediation plans fail because nobody asked whether the fix was funded. Every entry has a dollar sign behind it, even if that dollar sign is "we need to request budget." That is how real remediation works.

### What I Would Do Differently
With more time and access, I would expand the assessment to 12-15 controls covering backup, incident response, and physical security. I would add quantitative risk scoring (FAIR methodology) instead of qualitative High/Medium/Low. I would build a vendor registry with automated reassessment triggers. This portfolio represents a focused five-control assessment. A production engagement would be broader. I am aware of the difference.

## Contact

- Email: brandon@bnmsec.com
- LinkedIn: linkedin.com/in/brandon-schuerenberg
- Website: bnmsec.com
