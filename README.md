#  Medical Appointment No Shows – Data Cleaning task

This task focuses on cleaning and preprocessing the "Medical Appointment No Shows" dataset from Kaggle. The dataset contains over 110,000 records of medical appointments and whether or not the patients showed up.

---

## Dataset Summary

- Source: [Kaggle – No Show Appointments](https://www.kaggle.com/datasets/joniarroba/noshowappointments)
- Original Rows: 110,528  
- Final Cleaned Rows: 110,527

---

##  Data Cleaning Steps

###  Duplicates
- Checked for duplicates across all columns
-  No duplicate rows found

###  Age Column
- Found 1 negative age value → removed
- Found multiple `Age = 0` entries →  unclear if valid, so replaced with blanks

###  Categorical Fields
- `gender` standardized to `F` and `M`
- `no_show` converted to uppercase: `YES` / `NO`

###  Date Columns
- `scheduled_day` and `appointment_day` were converted to consistent ISO date format (`DD-MM-YYYY`)

### Column Names
- All column names converted to `lowercase`
  - Example: `ScheduledDay` → `scheduled_day`

###  Missing Values
- Found 1 row with all values missing →  removed
- `age` had 3540 blank values after replacing zeros

---

##  Files in This Repo

- `KaggleV2-May-2016_cleaned.xlsx` – Cleaned Excel dataset
- `README.md` – This summary of the data cleaning process

---

##  Key Learnings

- Real-world datasets often contain noise like missing or invalid values
- Standardization and consistency are critical for reliable analysis
- Data cleaning is as important as the analysis itself.

---

##  Useful Links

- [Original Dataset on Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments)
- [Project Contributor: Your Name Here](#)

---


