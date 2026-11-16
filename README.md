\# Dental Insurance Claims \& Actuarial Analytics (SQL + Python)



An end-to-end healthcare and actuarial analytics portfolio built on a synthetic 4-year (2021–2024) dental insurance claims warehouse. This project demonstrates complex SQL data modeling (SCD Type 2 temporal joins, Gaps-and-Islands, multi-tier hierarchies, and cumulative lifetime accumulators) paired with Python statistical analysis.



\## Repository Architecture

\* \*\*`sql\_views/`\*\*: Production-grade SQL views standardizing net adjudication math (post-appeal and Coordination of Benefits), SCD2 plan history resolution, and 4-level provider hierarchy rollups.

\* \*\*`capstones/`\*\*: Four applied business case studies:

&#x20; 1. \*\*Group Risk Profiling \& Underwriting\*\*: Loss ratio volatility, non-calendar plan year anniversary resets, and DPPO plan-switching outcomes.

&#x20; 2. \*\*Provider Network \& FWA Audit\*\*: DSO vs. independent benchmarking, unbundling (`D0120`+`D0150`), multi-surface filling upcoding, and prior-auth anomalies.

&#x20; 3. \*\*Predictive Member Cost Modeling\*\*: Feature engineering annual vs. orthodontic lifetime accumulators in SQL to predict next-year claim severity in Python.

&#x20; 4. \*\*Experience Rating Reconstruction\*\*: Rebuilding 3-year group renewal pricing by isolating `expense\_pepm` loads and post-appeal claim experience.



\## Quickstart (Local Setup)

1\. Clone this repository and install Python dependencies:

&#x20;  ```bash

&#x20;  pip install -r requirements.txt

&#x20;  ```

2\. Place your local copy of `dental\_claims.db` in the root directory \*(excluded from version control per data license)\*.

3\. Execute the reusable views in `sql\_views/` before running the Capstone notebooks/scripts.



\## Data Attribution \& Disclaimer

> \*\*Data:\*\* Dental Claims Synthetic Dataset (v2.0), a computer-generated educational dataset.  

> \*Note: All member, provider, employer group, and claim records are synthetic. Raw database files are excluded from this repository in compliance with the dataset usage agreement.\*



