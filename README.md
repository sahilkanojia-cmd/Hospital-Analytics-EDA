# 🏥 Hospital Analytics & Exploratory Data Analysis

## 📌 Project Overview

This project focuses on performing an end-to-end **Hospital Analytics and Exploratory Data Analysis (EDA)** using multiple interconnected healthcare datasets such as:

- Departments
- Doctors
- Patients
- Appointments
- Admissions
- Billing
- Lab Tests

The project covers the complete data analysis workflow, starting from understanding raw data and data quality issues to cleaning, standardization, data integration, feature engineering, exploratory analysis, and generating meaningful business insights.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Understand hospital operational and patient-related data
- Identify and handle data-quality issues
- Clean and standardize multiple datasets
- Check relationships between interconnected tables
- Combine datasets using appropriate keys
- Analyze hospital admissions and patient outcomes
- Analyze billing and insurance patterns
- Evaluate appointment performance
- Analyze laboratory test results
- Identify important trends and patterns
- Generate actionable business insights

---

## 📂 Dataset Structure

The project uses multiple interconnected datasets:

| Dataset | Description |
|---|---|
| Departments | Hospital department information |
| Doctors | Doctor and department information |
| Patients | Patient demographic and insurance information |
| Appointments | Appointment details, waiting time, status and satisfaction |
| Admissions | Hospital admission and patient-care information |
| Billing | Hospital billing and payment information |
| Lab Tests | Laboratory test results and costs |

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**
- **Git & GitHub**

---

## 🔄 Project Workflow

### 1. Data Understanding

- Loaded all datasets
- Examined dataset shape and structure
- Checked column names and data types
- Reviewed unique values
- Identified missing values
- Checked duplicate records

### 2. Data Cleaning

The datasets were cleaned and standardized by:

- Handling missing values
- Removing duplicate records
- Standardizing categorical values
- Converting columns to appropriate data types
- Checking inconsistent values
- Validating key columns

### 3. Data Integration

The interconnected datasets were combined using appropriate keys such as:

- `patient_id`
- `doctor_id`
- `department_id`
- `admission_id`
- `appointment_id`

Foreign-key relationships were checked to ensure data consistency.

### 4. Feature Engineering

Several analytical features were created, including:

- **Length of Stay**
- **Patient Payable**
- **Coverage %**
- **Cost per Day**
- **Age Group**

These features were used for deeper analysis.

---

# 📊 Exploratory Data Analysis

## 1. Department Analysis

Department-level analysis was performed to understand:

- Admission distribution
- Department revenue
- Average billing
- Doctor workload
- Outstanding payments

General Medicine and Cardiology contribute strongly to overall hospital revenue, while department-wise average billing remains relatively similar.

---

## 2. Billing & Insurance Analysis

The analysis examined:

- Total hospital billing
- Patient payable amount
- Insurance coverage
- Payment status
- Outstanding payments
- Insurance type

Private insurance accounts for the largest share of patients.

Outstanding payments were particularly concentrated in departments such as **General Medicine, Oncology, and Gynecology**, highlighting areas where payment collection may require greater attention.

---

## 3. Patient Care Analysis

Patient-care analysis included:

- Length of stay
- Diagnosis
- Admission type
- Patient outcomes
- Age groups
- Room types

Most patients have relatively similar lengths of stay across diagnoses, although some diagnoses show high-length-of-stay outliers.

**Recovered** patients represent the largest outcome category across age groups, followed by **Improved** patients.

---

## 4. Appointment Analysis

Appointment analysis focused on:

- Appointment types
- Waiting time
- No-show rate
- Cancellation rate
- Satisfaction score
- Department-wise waiting time

Average waiting times are fairly similar across departments.

**Radiology recorded the longest average waiting time at 24.35 minutes.**

Appointment no-show and cancellation rates were also relatively consistent across appointment types.

---

## 5. Laboratory Test Analysis

Laboratory data was analyzed using:

- Test type
- Result values
- Result flags
- Test cost
- Abnormal rates

### Abnormal Rate Findings

| Lab Test | Abnormal Rate |
|---|---:|
| Blood Sugar | **20.25%** |
| Creatinine | 20.12% |
| Cholesterol | 19.92% |
| Hemoglobin | 19.44% |
| Platelets | 19.35% |
| WBC Count | 19.19% |

**Blood Sugar recorded the highest abnormal rate at 20.25%.**

---

# 💡 Key Business Insights

### 🏥 Department Performance

General Medicine and Cardiology contribute strongly to overall hospital revenue. However, average billing across departments is relatively similar, suggesting that revenue is distributed fairly evenly.

### 💰 Billing & Insurance

Private insurance represents the largest share of patients. Outstanding payments are concentrated in several departments, indicating potential opportunities for improving payment collection.

### 👨‍⚕️ Patient Care

Recovered patients form the largest outcome category. Length of stay is generally similar across diagnoses, although certain diagnoses contain high-length-of-stay observations.

### 📅 Appointments

Radiology has the longest average waiting time at **24.35 minutes**. Routine Checkup has the highest no-show rate at **10.26%**, while Consultation has the highest cancellation rate at **12.09%**.

### 🧪 Laboratory Tests

Blood Sugar has the highest abnormal rate at **20.25%**, while WBC Count has the lowest at **19.19%**.

---

# 📈 Key Visualizations

The project includes visualizations covering:

- Department Performance
- Department Revenue
- Admission Type Distribution
- Room Type Distribution
- Patient Outcomes
- Payment Status
- Insurance Type
- Length of Stay vs Total Bill
- Monthly Admissions & Revenue
- Appointment No-Show & Cancellation Rate
- Department Waiting Time
- Lab Test Abnormal Rate

Visualizations are available in the `visuals/` folder.

---

# 📁 Project Structure

```text
Hospital-Analytics-EDA/
│
├── data/
│   ├── departments.csv
│   ├── doctors.csv
│   ├── patients.csv
│   ├── appointments.csv
│   ├── admissions.csv
│   ├── billing.csv
│   └── lab_tests.csv
│
├── notebook/
│   └── Hospital_Analytics_EDA.ipynb
│
├── visuals/
│   ├── appointment_no_show_cancellation.png
│   ├── lab_abnormal_rate.png
│   ├── department_revenue.png
│   ├── monthly_admissions_revenue.png
│   └── ...
│
├── README.md
└── requirements.txt
