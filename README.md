# Healthcare Readmission Risk Simulation

### Modeling Realistic Hospital Readmission Patterns with Python

## Overview

This project simulates realistic hospital patient encounter data to model and analyze readmission patterns.

Using Python (`pandas`, `numpy`, `matplotlib`), I generated a synthetic dataset of 10,000+ patient records that reflects real-world healthcare dynamics, including utilization behavior and clinical testing patterns.

The goal was to create a controlled environment where readmission risk factors can be explored, validated, and visualized without relying on protected health data.

---

## Objectives

* Simulate realistic patient encounter data based on known healthcare patterns
* Model relationships between utilization (inpatient, outpatient, emergency visits) and readmission risk
* Validate that simulated data behaves similarly to real-world trends
* Create a reusable dataset for downstream analysis and workflow testing

---

## Key Concepts Modeled

* Age-based patient segmentation
* Inpatient, outpatient, and emergency utilization patterns
* A1C testing and diabetes-related indicators
* Readmission outcomes (binary classification)
* Risk amplification based on prior utilization

---

## Methodology

### 1. Data Generation

* Created 10,000+ synthetic patient records using `numpy` random distributions
* Structured variables to mirror real clinical datasets:

  * Age groups
  * Encounter counts (inpatient, outpatient, emergency)
  * Lab testing indicators (A1C, glucose)
  * Readmission status

### 2. Probabilistic Modeling

* Applied weighted probability logic to simulate real-world risk dynamics
* Example:

  * Higher inpatient visit counts → increased probability of readmission
  * Certain utilization patterns → elevated risk profiles

This allowed the dataset to behave more like actual hospital data rather than purely random noise.

### 3. Data Processing

* Used `pandas` for:

  * Data structuring
  * Feature creation
  * Validation checks
  * Aggregation and grouping

### 4. Validation & Visualization

* Built visual checks using `matplotlib` to confirm expected trends:

  * Readmission rates vs inpatient utilization
  * Age distribution patterns
  * Utilization frequency distributions

These visualizations ensured the simulation produced realistic and interpretable outputs.

---

## Example Insights

* Patients with higher inpatient utilization showed significantly increased simulated readmission rates
* Age distribution influenced overall risk patterns and utilization behavior
* Simulated data successfully reproduced expected directional trends seen in clinical datasets

---

## Tools Used

* Python
* pandas
* numpy
* matplotlib
* Jupyter Notebook

---

## Project Structure

```
/data_generation.py      # Core simulation logic  
/analysis.ipynb         # Exploration and validation  
/visualizations/        # Output plots  
/README.md  
```

---

## Why This Project Matters

Real-world healthcare data is often restricted due to privacy concerns.

This project demonstrates how synthetic data can be used to:

* Prototype analyses
* Test workflows
* Explore risk models
* Build reproducible analytics pipelines

It also reflects my experience working with clinical data in a CAP-regulated environment, where data integrity and realistic interpretation are critical.

---

## Future Improvements

* Introduce time-series encounter modeling
* Add comorbidity variables for more complex risk modeling
* Build a predictive model (logistic regression / ML) on top of the simulated data
* Export dataset for use in SQL/Tableau dashboards

---

## Author

**Jarin Dengler**

* GitHub: https://github.com/jarindengler
* LinkedIn: [www.linkedin.com/in/jarindengler](http://www.linkedin.com/in/jarindengler)

---
