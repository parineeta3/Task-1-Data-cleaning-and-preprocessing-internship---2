🧹 Data Cleaning and Preprocessing – Medical Appointment No Shows Dataset

📘 Project Overview

This project is part of a Data Analyst Internship Task 1, focusing on data cleaning and preprocessing using Python (Pandas).
The dataset used is the Medical Appointment No Shows Dataset from Kaggle, which contains information about medical appointments in Brazil and whether patients showed up for their scheduled appointments.

🎯 Objective

To clean and prepare the raw dataset by:

Handling missing values

Removing duplicate records

Standardizing text values

Correcting data types (e.g., date, integers)

Renaming columns to a clean and uniform format

🧰 Tools & Libraries Used

Python

Pandas

Google Colab

📂 Dataset Details

Dataset Name: Medical Appointment No Shows

Source: Kaggle
Rows: ~110,000
Columns: 14
Target Variable: No-show (Yes/No)

Key Columns:

PatientId, AppointmentID, Gender, ScheduledDay, AppointmentDay, Age, Neighbourhood, Scholarship, Hipertension, Diabetes, Alcoholism, Handcap, SMS_received, No-show

🧩 Data Cleaning Steps

Loaded Dataset: Imported the raw CSV file into Python using Pandas.

Checked Null Values: Verified missing values using df.isnull().sum() and filled accordingly.

Handled Missing Values: Replaced missing numeric data with median values and text data with “Unknown”.

Removed Duplicates: Dropped duplicate rows using df.drop_duplicates().

Standardized Text Data:

Cleaned spaces and casing in Gender, Neighbourhood, and No-show.

Unified responses (Yes/No format).

Converted Data Types:

Converted ScheduledDay and AppointmentDay to datetime format.

Ensured numeric columns like Age, Scholarship, Diabetes are of integer type.

Renamed Columns:

Applied uniform lowercase and underscores using

df.columns = df.columns.str.lower().str.replace(' ', '_').str.replace('-', '_')


Saved Cleaned Data:

Exported the final dataset as Medical_Appointment_NoShows_Cleaned.csv.

📊 Results

All columns cleaned and standardized.

No missing or duplicate records remaining.

Ready-to-use dataset for analysis or visualization.

Final File: Medical_Appointment_NoShows_Cleaned.csv

💡 Learnings

Practical experience in identifying and resolving common data quality issues.

Improved understanding of data preprocessing before analysis.

Hands-on use of Pandas functions for real-world data cleaning.

👩‍💻 Author

Name: Parineeta Jagratt
Role: Data Analyst Intern
Tools Used: Google Colab, Pandas, NumPy
Task Type: Internship Task 1 – Data Cleaning & Preprocessing
