# CDISC SDTM Conversion Pipeline

Converting raw clinical trial data to standardized CDISC SDTM format for regulatory submissions.

## Project Overview

This project demonstrates the end-to-end process of transforming raw clinical study data into CDISC SDTM datasets that meet FDA regulatory requirements. The work follows SDTM Implementation Guide v3.2 specifications.

## Current Status

Project setup complete with reference data in place. Domain conversion programs in development.

## SDTM Domains

Building seven core SDTM domains:

- **DM** - Demographics
- **VS** - Vital Signs
- **LB** - Laboratory Results
- **AE** - Adverse Events
- **EX** - Treatment Exposure
- **MH** - Medical History
- **CM** - Concomitant Medications

## Project Structure

```
sdtm-conversion-pipeline/
├── data/
│   ├── raw/          # Source clinical data
│   ├── sdtm/         # Output SDTM datasets
│   └── reference/    # CDISC pilot data for validation
├── programs/         # SAS conversion programs
├── specs/            # Data mapping specifications
├── validation/       # QC and validation scripts
└── metadata/         # Dataset definitions
```

## Technical Approach

**Tools:** SAS Programming
**Standards:** CDISC SDTM IG v3.2
**Reference Data:** CDISC Pilot Study (CDISCPILOT01)
**Validation:** Pinnacle 21 Community

## Data Sources

Reference datasets from the official CDISC SDTM/ADaM Pilot Project are used for structure validation and quality control. All working data is synthetic.

## Implementation

Each SDTM domain will be created through:
1. Data mapping from raw to SDTM structure
2. Variable standardization and controlled terminology application
3. ISO 8601 date formatting
4. Cross-domain consistency checks
5. Validation against CDISC specifications

## Quality Control

- Adherence to SDTM variable naming conventions
- Controlled terminology verification
- Missing data handling
- Cross-domain referential integrity
- Pinnacle 21 validation

---

**Author:** Venkata Akhil Mettu
**Standards Compliance:** CDISC SDTM IG v3.2
