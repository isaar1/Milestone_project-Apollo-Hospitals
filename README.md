# Apollo Hospitals - Appointment No-Show and Patient Engagement Analysis

## Objective
Find out why patients miss appointments and how Apollo can reduce no-shows, using exploratory data analysis in Python.

## Dataset
Included in the `Datasets` folder:
- apollo_appointments_fact.csv: 75,000 appointments (2022-2024), 52 columns
- apollo_doctors_dim.csv: 320 doctors, 15 columns
- Data Dictionary.docx: description of every column

## Approach
- Cleaned and checked the data (duplicates, dates, ranges)
- No-show rate = No-Shows / (Completed + No-Show + Cancelled), excluding Scheduled
- Revenue and service quality analysis uses Completed appointments only
- Analysed business overview, no-show drivers, reminders, patient segments, finance and doctor utilisation

## Key Findings
- Overall no-show rate is 15.94%, about 1 in 6 booked appointments
- No-shows cost an estimated 15.7M to 19.7M, about 21% of revenue earned
- First-time patients: 66.8% no-show vs 8.6% for repeat patients
- No reminder: about 30% no-show, falling to about 11% with three reminders
- Prior no-shows and long lead time (15-30 days) raise the risk

## Recommendations
1. Send at least one reminder to every booking
2. Call first-time patients and patients with 2 or more prior no-shows
3. Add extra reminders for Home Visit and Video Consult bookings
4. Plan doctor capacity around the Q4 and Q1 peak

## How to Run
1. Download or clone this repository
2. Install the libraries: pandas, numpy, matplotlib, seaborn, jupyter
3. Open `Apollo_No_Show_Analysis.ipynb` and choose Run All