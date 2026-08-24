# MASLD-Phenotyping
MASLD Phenotyping Using Unsupervised Machine Learning
## Overview

**Metabolic dysfunction-associated steatotic liver disease (MASLD)**, previously known as **non-alcoholic fatty liver disease (NAFLD)**, is a form of steatotic liver disease characterized by excess fat accumulation in the liver in the presence of cardiometabolic risk factors such as obesity, dysglycemia, hypertension, and dyslipidemia.

Because these metabolic abnormalities can occur in different combinations and severities, MASLD is a **heterogeneous condition**. This project uses **unsupervised machine learning** to determine whether individuals in a MASLD cohort can be grouped into distinct phenotypic patterns based on their clinical and metabolic characteristics.
 ## MASLD Disease Spectrum

<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41423-025-01307-5/MediaObjects/41423_2025_1307_Fig1_HTML.png" alt="MASLD disease spectrum" width="650"/>

*Figure adapted from He et al., 2025, Cellular & Molecular Immunology, licensed under CC BY 4.0. The figure illustrates the progression of MASLD from steatosis through hepatitis, cirrhosis and liver cancer, and highlights metabolic and genetic factors involved in disease progression.*

## What Was Analyzed?

Nine clinical and metabolic variables were used for clustering:

**Age, BMI, HbA1c, ALT, LDL, triglycerides, waist circumference, systolic blood pressure, and fasting glucose.**

Multiple unsupervised clustering approaches were compared, including PAM, K-means, and Fuzzy C-means, with cluster number, agreement, and stability evaluated.

## Key Findings

The final analysis included **350 participants** and supported a **three-cluster structure**.

* **Cluster 1 (n = 197):** Older participants with relatively lower BMI, waist circumference, and fasting glucose.
* **Cluster 2 (n = 84):** Higher BMI, waist circumference, and LDL, representing an **adiposity–lipid pattern**.
* **Cluster 3 (n = 69):** Higher BMI, waist circumference, fasting glucose, and HbA1c, representing an **adiposity–glycemic pattern**.

Overall, the analysis reveals **different combinations of metabolic characteristics within MASLD**, rather than a single uniform metabolic profile.

Cluster stability was assessed using **1,000 repeated 80% subsampling iterations**, with a mean ARI of **0.679**.

## Repository Contents

* `MASLD_Phenotyping.Rmd` — R Markdown source and complete analysis
* `MASLD_Phenotyping.html` — rendered analysis report
* `MASLD_PRINT.pdf` — PDF report
* `LICENSE` — MIT License

## Data

Participant-level data are not included in this repository.

## License

This project is released under the **MIT License**.

## Author

**Rushikesh Jadhav**
