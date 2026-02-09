# Cancer Outcomes Intelligence System (COIS)
## Requirements Analysis

### 1. Purpose
Build a data engineering–led system to analyze breast cancer outcomes for clinical research.
This system supports population-level research, not diagnosis or treatment decisions.

### 2. Primary User
Clinical researchers studying cancer survival outcomes.

### 3. Research Questions
RQ1: How does overall survival vary by stage at diagnosis?
RQ2: How do treatment categories relate to survival outcomes?
RQ3: How do survival trajectories differ across demographic groups?

### 4. Scope
- Disease: Breast cancer
- Outcome: Overall survival
- Timeline: Diagnosis → death or censoring

### 5. Inclusion Criteria
- First primary breast cancer
- Known diagnosis date
- Known survival time or censoring status
- Adult patients

### 6. Exclusion Criteria
- Multiple primary cancers
- Missing key dates
- Pediatric cases
- Rare subtypes (v1)

### 7. Assumptions & Limits
- Data is observational
- Associations ≠ causation
- Results are research-only

### 8. Success Criteria
- Clean, reproducible dataset
- Valid survival curves
- Clearly documented insights and limits
