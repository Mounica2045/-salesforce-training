# Day 3 – Data Modeling

## Why do companies need structured data instead of random spreadsheets?

Companies handle huge amounts of information such as employee details, customer records, sales, inventory, attendance, and payments. Random spreadsheets create problems like duplicate data, missing information, confusion, and security issues.

Structured data helps companies:
- Store data in an organized way
- Reduce errors and duplication
- Improve security and access control
- Generate reports easily
- Maintain relationships between data
- Scale operations efficiently

Example:
Instead of storing student data in many separate Excel sheets, a college management system stores everything in connected tables/objects like Students, Faculty, Courses, and Attendance.

---

# 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|----------|----------|
| App | Collection of tools/modules used for a specific purpose | College Management App |
| Object | A table that stores similar types of data | Student Object |
| Record | A single row of data inside an object | One student's details |
| Field | A single attribute/column in a record | Student Name |

### Example

Student Object:

| Student ID | Name | Branch |
|------------|------|--------|
| 101 | Mounika | CSE |

- Object = Student
- Record = Row containing Mounika’s data
- Field = Name / Branch / Student ID
- App = Entire College Management System

---

# 2. Standard vs Custom Objects

| Standard Objects | Custom Objects |
|------------------|----------------|
| Pre-built objects provided by the platform | User-created objects |
| Commonly used in all systems | Created for specific business needs |
| Example: User, Account | Example: Hostel, Library Book |

### Examples

### Standard Objects
- User
- Employee
- Account

### Custom Objects
- Student
- Faculty
- Attendance
- Hostel Room

---

# 3. College Data Model

## Objects

1. Student
2. Faculty
3. Course
4. Department
5. Attendance

---

## Relationships

- One Department has many Students
- One Faculty teaches many Courses
- One Student attends many Courses
- Attendance belongs to both Student and Course

---

## Data Model Diagram

```text
Department
    |
    | 1:M
    |
Student -------- Attendance -------- Course
                      |
                      |
                   Faculty

4. Formula Fields

Formula fields automatically calculate values using existing data.

Example 1: Student Percentage
Percentage = (Marks Obtained / Total Marks) * 100
Explanation

This formula automatically calculates the student's percentage.

Example 2: Attendance Percentage
Attendance % = (Classes Attended / Total Classes) * 100
Explanation

This formula helps track student attendance automatically.

Example 3: Grade Calculation
IF Percentage >= 90 → Grade A
IF Percentage >= 75 → Grade B
ELSE Grade C
Explanation

Grades are automatically assigned based on percentage.

5. Validation Rules

Validation rules ensure correct and valid data entry.

Example 1: Phone Number Validation
Phone number must contain exactly 10 digits.
Explanation

Prevents invalid phone numbers from being saved.

Example 2: Attendance Validation
Attendance cannot exceed total classes.
Explanation

Stops incorrect attendance entries.

Example 3: Email Validation
Email must contain '@'
Explanation

Ensures proper email format.

6. Reflection – Why Structured Enterprise Data Matters

Structured enterprise data is very important because organizations depend on accurate and connected information for decision-making. Proper data modeling improves efficiency, reduces mistakes, increases productivity, and helps businesses grow.

Without structured data:

Data becomes inconsistent
Reports become inaccurate
Duplicate records increase
Managing information becomes difficult

With structured data:

Data is organized and secure
Systems become scalable
Reports and analytics become easy
Teams can collaborate efficiently

Therefore, structured data is the foundation of modern enterprise applications and business systems.
<img width="1903" height="907" alt="Screenshot 2026-05-09 204346" src="https://github.com/user-attachments/assets/ed51d584-98bc-486d-a04e-e98692758de6" />
<img width="792" height="486" alt="Screenshot 2026-05-09 175005" src="https://github.com/user-attachments/assets/660b3bf0-fd51-42e2-9cc9-eb4de07c2bad" />
<img width="1903" height="901" alt="Screenshot 2026-05-07 234040" src="https://github.com/user-attachments/assets/c8b471cf-323e-4175-9d80-ab00a715cbe5" />
<img width="1900" height="924" alt="Screenshot 2026-05-07 232631" src="https://github.com/user-attachments/assets/80cbee46-f0b6-4179-b02f-ca8ca53497e8" />
<img width="1903" height="911" alt="Screenshot 2026-05-07 233830" src="https://github.com/user-attachments/assets/a9c4f05f-28a5-46cb-9b79-199b0d8826aa" />

