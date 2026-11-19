# student-enrollment-performance-dashboard
Power BI dashboard analysing student enrollments, scores and programs: data cleaning in Power Query, DAX measures, charts and a program slicer.

# Student Enrollment & Performance Dashboard

A Power BI project analysing student enrollments and performance across courses and programs.
![Dashboard](screenshots/dashboard.png)

## Project overview
The dashboard shows how many students enrolled in each course, how well they scored, and how students are spread across programs. A Program slicer lets the viewer filter the whole report.

## Key numbers
- **Total enrollments:** 39
- **Total students:** 22
- **Average score:** 79.08

## What I did
1. **Data cleaning in Power Query**
   - Checked data types: Age (Students), Enrollment_Date (Enrollments), Score and Attendance_Rate (numeric)
   - Removed duplicate records
   - Removed rows with missing values
   - Renamed columns where needed, then loaded the cleaned data into Power BI
2. **DAX measures**: Total Enrollments (count of enrollment records), Average Score, Total Students
3. **Visuals**: enrollments by course, average score by course, students by program, plus a Program slicer

## Findings
- *Introduction to Data Analytics* has the most enrollments (6), while *SQL Fundamentals* has the fewest (1).
- *Introduction to Data Analytics* and *Power BI for Reporting* have the highest average scores.
- Students are spread fairly evenly across programs: Business Administration, Computer Science and Data Analytics have 6 each, and Information Technology has 4.

## Data
Three practice tables, linked by ID columns:
- **Students**: Student_ID, Student_Name, Gender, Age, City, Program
- **Courses**: Course_ID, Course_Name, Department, Instructor, Course_Level
- **Enrollments**: Enrollment_ID, Student_ID, Course_ID, Enrollment_Date, Score, Attendance_Rate, Status
The files in `data/` are the original raw versions, before cleaning.

## Files
- `data/`: the three source tables
- `screenshots/`: image of the dashboard

## Skills used
Power BI, Power Query, data cleaning, DAX measures, data visualization, slicers
