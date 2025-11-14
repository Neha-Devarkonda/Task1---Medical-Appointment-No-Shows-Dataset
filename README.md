Summary of Task 1
Data Cleaning Task (Medical Appointment No Shows Dataset)
📌 Objective

The goal of this task is to clean and prepare a raw dataset containing missing values, duplicates, inconsistent text formats, incorrect data types, and unstructured date fields. The dataset used for this task is Medical Appointment No Shows (Kaggle).

🛠️ Tools Used

Python (Pandas)
Google Colab - Notebook
(Excel can also be used)

📂 Dataset

Name: Medical Appointment No Shows

Source: Kaggle

Description: Contains patient details, appointment information, and a target column indicating whether the patient showed up for their medical appointment.

🔧 Cleaning Steps Performed
1.Uploded dataset file (/content/noshowappointments.csv)

2. Missing Values

Checked missing values using df.isnull().sum().

Filled missing Age with median.

Filled missing Gender with mode.

Removed rows with missing appointment dates.

2. Duplicate Records

Identified and removed duplicate rows using df.drop_duplicates().

3. Standardized Text Fields

Converted all text to lowercase and stripped extra spaces.

Standardized values in:

Gender → male, female

No-show → yes, no

4. Date Format Cleaning

Converted ScheduledDay and AppointmentDay to consistent format (dd-mm-yyyy).

Ensured proper datetime data types.

5. Column Name Cleanup

Renamed columns to lowercase, snake_case format
(example: ScheduledDay → scheduled_day)

6. Data Type Corrections

Converted Age to integer.

Converted date columns to datetime.

Set no-show column as category type.

7. Invalid Data Handling

Removed records with negative or unrealistic ages (less than 0 or greater than 120).

📤 Output

Cleaned Dataset: /content/noshowappointments.csv
Dataset is ready for further analysis, visualization, or machine learning tasks.
