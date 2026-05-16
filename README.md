# Turbulence Load Stress Analysis in Wind Farm Telemetry

## Project Overview
This repository contains the **WindPowerMasterAnalyzer**, an Object-Oriented Programming (OOP) pipeline designed to process and analyze SCADA telemetry data from utility-scale wind farms. The study focuses on the relationship between atmospheric instability (Turbulence Intensity) and mechanical load stress, specifically addressing data integrity through automated anomaly detection and wind shear correction.

### Key Research Findings
- **Data Throughput:** Processed an initial master dataset of **175,200 records** across four geographical locations.
- **Anomaly Detection:** Successfully identified and purged **3,941 operational anomalies** using a heuristic-driven feature projection.
- **Correlation Enhancement:** Improved the Pearson Correlation Coefficient between 100m wind speed and power output to **r ≈ 0.96**.
- **System Stability:** Verified a global Mean Power Output of **0.3104 MW** with a moderate positive skewness of **0.7806**.

## About the Author
**John Emmanuel O. Genita** Student ID: **TUPM-25-3534** Department of Electronics Engineering  
Technological University of the Philippines (TUP), Manila  

This project was developed as part of the academic requirements for the **Electronics Engineering (ECE)** program, focusing on the intersection of data science, fluid mechanics, and structural health monitoring.

## Technical Stack
- **Language:** Python 3.x
- **Libraries:** NumPy, Pandas, SciPy, Matplotlib/Seaborn
- **Framework:** Object-Oriented Programming (OOP)
- **Data Sources:** Multi-site SCADA Telemetry (CSV)

## Core Methodology
The system architecture follows a sequential four-stage workflow:
1. **Data Ingestion:** Robust multi-file integration using `try-except` blocks.
2. **Purification:** Boolean masking to eliminate null values and "high wind/zero power" states.
3. **Analytics:** Vectorized computation of statistical moments (Mean, Variance, Skewness).
4. **Visualization:** Mapping of power-curve trajectories and anomaly clustering.