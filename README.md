# Healthcare Data Analysis with Power BI

## Overview

This project involves a comprehensive analysis of healthcare datasets using Power BI. The goal is to uncover trends and insights that can improve patient outcomes and optimize hospital operations. By integrating data cleaning, sophisticated data modeling, and DAX for advanced analytics, an interactive dashboard has been created to visualize key aspects of the healthcare data.

This analysis was conducted as part of a case study for HealthStat Solutions, a company specializing in healthcare analytics.

## Data Sources

The analysis utilizes two datasets provided in Excel format:

1.  **HealthcareDataset1.xlsx**: Contains detailed patient information, including demographics, diagnosis, treatment, admission/discharge dates, total bills, and prescription details.
2.  **HealthcareDataset2.xlsx**: Provides hospital treatment details, such as the treating doctor, room number, daily costs, treatment types, and recovery ratings, linked to patients via `PatientID`.

These datasets can be found at the following links:

* [HealthcareDataset1.xlsx](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42c5605803a0/f612ea2d-d0ea-4f03-9d9e-056baa3a6658/HealthcareDataset1.xlsx)
* [HealthcareDataset2.xlsx](https://prod-files-secure.s3.us-west-2.amazonaws.com/d1e1bc70-9ede-4c69-84fd-42d-f75a0affd3d7/HealthcareDataset2.xlsx)

## Data Preparation

1.  **Merging Datasets:** The `HealthcareDataset1.xlsx` and `HealthcareDataset2.xlsx` datasets were merged in Power BI using the `PatientID` as the key to combine patient information with hospital treatment details.

2.  **Data Preprocessing:** After merging, the following preprocessing steps were performed:
    * Blank values in the 'PatientName' column were replaced with 'Unknown'.
    * Blank values in the 'Hospital' column were replaced with 'Unknown'.
    * The data types of the 'AdmissionDate' and 'DischargeDate' columns were converted to datetime format.
    * Missing values in the 'RecoveryRating' column were imputed using the average recovery rating.

## Key Insights from the Analysis

The Power BI dashboard and underlying analysis revealed several important trends and insights, including:

* **Patient Demographics:** The predominant age groups are Senior and Adult.
* **Treatment Costs:** Surgery has the highest average treatment cost.
* **Diagnosis by Gender:** Some variations in gender distribution across different diagnoses were observed.
* **Blood Type Prevalence:** AB+ and B- are among the most prevalent blood types.
* **Recovery Rating:** Counseling has the highest average recovery rating by treatment type.
* **Hospital Utilization:** Green Valley Medical Center shows the highest average number of patients per room.
* **Doctor Impact:** The treating doctor significantly influences the average recovery rating.
* **Cost vs. Recovery:** No strong correlation was found between total treatment cost and recovery rating.
* **Age and Recovery:** No strong linear correlation was observed between patient age and recovery rating.
* **Hospital Performance:** Riverside Hospital showed a high average recovery rating with a lower average treatment cost.

## Power BI Dashboard

The interactive Power BI dashboard provides a comprehensive view of the healthcare data, featuring:

* **Key Performance Indicators (KPIs):** Total Patients, Number of Hospitals, Average Recovery Rating, Total Treatment Cost, and Average Daily Cost.
* **Patient Demographics:** Distribution of patients by age group and blood type.
* **Treatment Analysis:** Number of patients by treatment type and average treatment costs.
* **Hospital Performance:** Metrics such as patient load, average treatment cost, and average recovery rating per hospital.
* **Diagnosis Trends:** Distribution of diagnoses across hospitals.
* **Temporal Analysis:** Patient counts by month.
* **Interactive Filtering:** Slicers for Year, Gender, Age Group, Diagnosis, Hospital, and Treatment to allow users to explore specific subsets of the data.

## Conclusion

This healthcare data analysis successfully leveraged Power BI to process, model, and visualize key aspects of patient records and hospital treatment details. The resulting dashboard offers valuable insights into patient demographics, treatment effectiveness, hospital performance, and potential areas for improvement in healthcare delivery and operational efficiency. The findings can aid healthcare providers in making more informed decisions to enhance patient care and optimize resource allocation.

---
