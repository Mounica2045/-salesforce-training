# 1. What is Salesforce Platform?

The Salesforce Platform is a **cloud-based application development platform** that allows businesses to create, customize, and manage applications without managing hardware or infrastructure.

It provides:

* Database services
* Security
* Automation
* User interface
* Reporting
* APIs
* App development tools

Salesforce follows:

* SaaS (Software as a Service)
* PaaS (Platform as a Service)
* Multi-tenant architecture

Developers and admins can build:

* CRM applications
* Business automation apps
* Employee management systems
* Customer service systems
* Custom enterprise applications

### Features

* Cloud-based access
* Easy customization
* Drag-and-drop tools
* Coding support using Apex and Lightning
* Automatic updates
* High security

### Official Resource

* [Salesforce Platform](https://www.salesforce.com/platform/?utm_source=chatgpt.com)

---

# 2. Explain

## A) App

An App in Salesforce is a collection of:

* Tabs
* Objects
* Reports
* Dashboards
* Features

grouped together for a specific business purpose.

### Example

Sales App may contain:

* Accounts
* Contacts
* Opportunities
* Reports

### Types of Apps

1. Standard Apps

   * Sales
   * Service
   * Marketing

2. Custom Apps

   * Student Management App
   * Library Management App
   * Hospital Management App

### Purpose

Apps help users access related functionalities in one place.

---

## B) Object

An Object in Salesforce is similar to a database table that stores data.

### Example

| Object                  | Stores               |
| ----------------------- | -------------------- |
| Account                 | Company details      |
| Contact                 | Customer information |
| Student (Custom Object) | Student records      |

### Types of Objects

### 1. Standard Objects

Provided by Salesforce:

* Account
* Contact
* Lead
* Opportunity

### 2. Custom Objects

Created by users according to business needs.

Example:

* Employee
* Student
* Course

### Object Contains

* Fields
* Records
* Relationships
* Validation rules

---

## C) Tab

A Tab is a user interface element used to access objects and features.

It helps users open:

* Object records
* Dashboards
* Reports
* Visual pages

### Example

* Student Tab → Opens Student records
* Report Tab → Opens reports

### Purpose

Tabs make navigation easy in Salesforce apps.

---

# 3. Difference: Configuration vs Coding

| Feature        | Configuration                         | Coding                        |
| -------------- | ------------------------------------- | ----------------------------- |
| Meaning        | Customization without programming     | Development using programming |
| Skill Required | Admin-level                           | Developer-level               |
| Tools Used     | Flow, Process Builder, Object Manager | Apex, Visualforce, LWC        |
| Complexity     | Simple to moderate                    | Complex logic                 |
| Speed          | Faster                                | Takes more time               |
| Maintenance    | Easier                                | Requires code maintenance     |
| Example        | Creating fields and workflows         | Writing Apex triggers         |

---

## Configuration Examples

* Creating objects
* Adding fields
* Validation rules
* Flows
* Page layouts

## Coding Examples

* Apex classes
* Apex triggers
* Lightning Web Components
* API integrations

---

# 4. Your System Design (App + Objects + User Interaction)

## Example: Student Management System

---

# A) App Name

**Student Management App**

Purpose:
Manage student records, courses, attendance, and faculty information.

---

# B) Objects

## 1. Student Object

Stores:

* Student ID
* Name
* Branch
* Email
* Phone

## 2. Course Object

Stores:

* Course Name
* Course ID
* Duration
* Faculty

## 3. Faculty Object

Stores:

* Faculty Name
* Department
* Qualification

## 4. Attendance Object

Stores:

* Student
* Date
* Status

---

# C) Relationships

* One Course → Many Students
* One Faculty → Many Courses
* One Student → Many Attendance Records

---

# D) Tabs

* Student Tab
* Course Tab
* Faculty Tab
* Attendance Tab
* Reports Tab

---

# E) User Interaction Flow

### Admin

* Creates courses
* Adds faculty
* Manages users

### Faculty

* Marks attendance
* Updates student performance

### Student

* Views attendance
* Checks course details

---

# F) Automation

Using Configuration:

* Attendance alerts
* Email notifications
* Validation rules

Using Coding:

* Custom attendance calculation
* Performance analytics

---

# G) Benefits

* Centralized data
* Easy tracking
* Cloud access
* Automated processes
* Secure management
<img width="778" height="656" alt="Screenshot 2026-05-09 174701" src="https://github.com/user-attachments/assets/db482d7a-505f-42e7-8107-aad683e2b9a4" />
<img width="775" height="434" alt="Screenshot 2026-05-09 174830" src="https://github.com/user-attachments/assets/9acef947-2541-4ebe-8a8a-47c7e2995010" />
<img width="773" height="448" alt="Screenshot 2026-05-09 174842" src="https://github.com/user-attachments/assets/85bb97ad-4630-41a2-b559-55e1af165823" />
<img width="782" height="669" alt="Screenshot 2026-05-09 174937" src="https://github.com/user-attachments/assets/3b22f303-511a-47ff-a08c-78381ab8e5af" />
<img width="780" height="528" alt="Screenshot 2026-05-09 174954" src="https://github.com/user-attachments/assets/ede37179-dfad-4b55-89d0-e9302b11b16e" />
<img width="792" height="486" alt="Screenshot 2026-05-09 175005" src="https://github.com/user-attachments/assets/6aa58d46-5fd2-47b0-b15a-dce89beb91be" />

