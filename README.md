# Project Title: Ladies in Tech Africa - Excel Functions

##  Table of Contents
- [Project Preview](#docs/project-preview.md)
- [Project Objective](#project-objective)
- [Project Significance](#project-significance)
- [Methodology](#methodology)
- [Prerequisites](#Prerequisities)
- [Discussion of Result](#discussion-of-result)

## Project Preview
This project, Ladies in Tech African Excel Project, aims to demonstrate the application of basic Excel functions and data analysis techniques using a sample dataset of worker salaries across different states in a company. The project will cover various Excel functions, including basic arithmetic functions, text cleaning, and VLOOKUP for salary structure.

## Project Objective
The primary objective of this project is to equip participants with the necessary skills to perform data analysis and management using Excel. By the end of this project, participants will be able to:

- Utilize basic and conditional functions in Excel.
- Clean and standardize text data.
- Extract specific information from text strings.
- Use lookup functions to retrieve and organize data.

 ## Project Significance
The significance of this project lies in its potential to empower women in Africa with valuable technical skills. Proficiency in Excel is crucial for data management and analysis in many industries, and this project aims to bridge the skill gap and enhance employability for women in tech.

## Methodology
The methodology for this project involves hands-on practice with Excel functions using a provided sample dataset. The project is divided into several sections, each focusing on different Excel functionalities:

### Basic Functions:
- SUM, AVERAGE, MAX, MIN, COUNT, LARGE, SMALL
- Text Cleaning:
- TRIM, UPPER, LOWER, PROPER, CONCATENATE, FIND, LEFT, MID, RIGHT
- VLOOKUP for Salary Structure:
- Using VLOOKUP to populate salary components based on employee level and department
- Each section will include explanations, examples, and practical exercises to reinforce learning.

## Prerequisites
- Basic knowledge of Excel.
- Access to a computer with Excel installed.
- The sample dataset was gotten from Ladies in Tech Africa, provided as part of this project.

## Discussion of Results
This project successfully demonstrates the effective utilization of Excel functions to manage and analyze data, showcasing proficiency in:
- Calculating total, average, maximum, and minimum salaries.
- Cleaning and standardizing text data for consistency.
- Combining and extracting names from email addresses.
- Utilizing VLOOKUP to organize and retrieve salary components based on employee level and department.

### Excel Function 1: Basic Functions
 ![excel1a](https://github.com/user-attachments/assets/13f476e3-80e2-4d77-9715-f052201e70ba)
### Calculations:

- Grand Total of Salaries: =SUM(D8:D27) → 56,165,334
- Average Salary: =AVERAGE(D8:D27) → 2,808,267
- Highest Salary: =MAX(D8:D27) → 56,165,334
- Lowest Salary: =MIN(D8:D27) → 1,130,642
- Total Number of Staff: =COUNT(D8:D27) → 20
- Fourth Highest Salary: =LARGE(D8:D27, 4) → 4,740,966.00
- Third Lowest Salary: =SMALL(D8:D27, 3) → 1,358,916.00

### Conditional Functions:
- Bayelsa Total Salary : =SUMIF(C8:C27,C11,D8:D27)
- Average Oyo Salary: =AVERAGEIF(C8:C27,C21,D8:D27)
- Highest Salary (Edo): =MAXIFS()
- Lowest Salary Taraba: =MINIFS()
- Total Number of Staff in Nasarawa: =COUNTIFS()

### Excel Function 2: Text Cleaning
Functions Used:

![excel2a](https://github.com/user-attachments/assets/bd93f9ac-b051-472d-8a03-16a957477451)
#### Name Cleaning
- Remove Unnecessary Spaces: =TRIM(B5)
- Removes leading, trailing, and excess spaces from the name in cell B5.
- Convert to Uppercase: =UPPER(B5)
- Converts the name in cell B5 to uppercase.
- Convert to Lowercase: =LOWER(B5)
- Converts the name in cell B5 to lowercase.
- Proper Case: =PROPER(B5)
- Capitalizes the first letter of each word in the name in cell B5.
- Proper Case & Trim: =PROPER(TRIM(B5))
- Combines proper case and trim functions.
  
  ![excel2b](https://github.com/user-attachments/assets/8aed2d05-9260-4f45-874e-74970517cd56)
#### Company Name Cleaning
- Proper Case: =PROPER(C5)
- Capitalizes the first letter of each word in the company name in cell C5.
  
![excel2c](https://github.com/user-attachments/assets/4c5d5c22-a33e-44b3-bfc4-6da09ddb4ef9)
#### Text Cleaning 3: Combining First & Last Names
- Formula: =B6 & " " & C6 or =CONCATENATE(B6, " ", C6)
-Combines first name (B6) and surname (C6) with a space.

![excel2d](https://github.com/user-attachments/assets/a5077adb-50d6-4f94-ad0f-94e6e9d53eb9)
#### Text Cleaning 4: Extracting Names from Email
First name from email: =LEFT(B6, FIND(".", B6)-1)
Surname from email: =MID(B6, FIND(".", B6)+1, FIND("@", B6)-1 - FIND(".", B6))

### Excel Function 3: VLOOKUP for Salary Structure
VLOOKUP was used to fill the table with salary components (Basic, Housing, Transportation, Leave, Meal, Utility, Gross) based on employee's level and department.

##### Reference Table (Simple Salary Structure):
![excel3b](https://github.com/user-attachments/assets/600be209-a8a1-4df8-9828-36697cb2d831)

#### VLOOKUP Formulas:
1. Basic: =VLOOKUP($E$9, $B$2:$I$16, 2, FALSE)
- Looks up value in cell E9 (employee level) in column B (Level) of the reference table.
- Returns value in column 2 (Basic).
2. Housing: =VLOOKUP($E$9, $B$2:$I$16, 3, FALSE)
- Returns value in column 3 (Housing).
3. Transportation: =VLOOKUP($E$9, $B$2:$I$16, 4, FALSE)
- Returns value in column 4 (Transportation).
4. Leave: =VLOOKUP($E$9, $B$2:$I$16, 5, FALSE)
- Returns value in column 5 (Leave).
5.  Meal: =VLOOKUP($E$9, $B$2:$I$16, 6, FALSE)
- Returns value in column 6 (Meal).
6. Utility: =VLOOKUP($E$9, $B$2:$I$16, 7, FALSE)
- Returns value in column 7 (Utility).
7. Gross: =VLOOKUP($E$9, $B$2:$I$16, 8, FALSE)
-Returns value in column 8 (Gross).
![excel3a](https://github.com/user-attachments/assets/04bbd54e-67cb-4b8a-b0f3-59af9497dbca)

## Conclusion
The Ladies in Tech African Excel Functions Project effectively demonstrates the capabilities of Excel in managing and analyzing data. By utilizing basic arithmetic functions, text cleaning techniques, and the VLOOKUP function, the project successfully processes and interprets a dataset of worker salaries.
The project's outcomes highlight a comprehensive understanding and application of Excel functions for data analysis and management, enabling:
- Calculation of total, average, maximum, and minimum salary values
- Cleaning and standardization of text data for consistency and accuracy
- Combination and extraction of specific information from text strings
- Effective use of VLOOKUP to retrieve and organize data based on employee levels
- These skills are essential for efficient data analysis and management, proving valuable in handling real-world data challenges. The project underscores the significance of - Excel proficiency in various professional fields and provides a practical framework for enhancing technical skills, ultimately showcasing readiness to leverage Excel expertise in professional settings.
