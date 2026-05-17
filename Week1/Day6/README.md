# Day 4 – SOQL, Apex Triggers & Automation

# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is a query language used in Salesforce to retrieve data from objects.

It is similar to SQL but designed specifically for Salesforce data.

### Example

```sql
SELECT Name, Branch__c FROM Student__c
```

### Explanation

This query retrieves the student name and branch from the Student object.

---

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of code that automatically executes when data changes occur in Salesforce objects.

Triggers can run:

* Before inserting data
* After inserting data
* Before updating
* After deleting

### Example Use

When a new student record is added, a trigger can automatically assign a student ID.

---

# 3. Difference Between

## Flow vs Trigger

| Flow                        | Trigger                        |
| --------------------------- | ------------------------------ |
| No-code/low-code automation | Code-based automation          |
| Easier for admins           | Used mainly by developers      |
| Simple business processes   | Complex logic handling         |
| Faster to build             | More powerful and customizable |
| Best for simple automations | Best for advanced automations  |

---

## Before Trigger vs After Trigger

| Before Trigger                  | After Trigger                             |
| ------------------------------- | ----------------------------------------- |
| Runs before data is saved       | Runs after data is saved                  |
| Used to validate or modify data | Used for related actions                  |
| Faster for field updates        | Used for sending emails, creating records |
| Example: Auto-fill values       | Example: Send notifications               |

---

# 4. Trigger Use Cases (5 Examples)

## 1. Auto Generate Student ID

When a new student record is created, the system automatically generates a unique student ID.

---

## 2. Attendance Alert

If attendance falls below 75%, automatically send a warning message.

---

## 3. Prevent Duplicate Email

Block saving records if the email already exists.

---

## 4. Update Course Count

When a student enrolls in a course, automatically update the total course count.

---

## 5. Send Welcome Email

After a student registers, automatically send a welcome email.

---

# 5. Query Examples (English Query Ideas)

## Example 1

Get all students from the CSE department.

### SOQL

```sql
SELECT Name FROM Student__c WHERE Branch__c = 'CSE'
```

---

## Example 2

Find students with attendance below 75%.

### SOQL

```sql
SELECT Name, Attendance__c FROM Student__c WHERE Attendance__c < 75
```

---

## Example 3

Get all faculty names teaching Python.

### SOQL

```sql
SELECT Name FROM Faculty__c WHERE Subject__c = 'Python'
```

---

## Example 4

Find students whose fees are pending.

### SOQL

```sql
SELECT Name FROM Student__c WHERE Fees_Status__c = 'Pending'
```

---

## Example 5

Show all courses offered by the CSE department.

### SOQL

```sql
SELECT Name FROM Course__c WHERE Department__c = 'CSE'
```

---

# 6. Reflection – Why Enterprise Systems React Automatically to Data Changes

Enterprise systems handle thousands of transactions daily. Manual monitoring is impossible. Automation helps systems react immediately whenever data changes occur.

Triggers and flows allow systems to:

* Update records automatically
* Send alerts instantly
* Maintain accurate data
* Reduce manual work
* Improve efficiency

For example, when attendance becomes low, the system can automatically notify students without human intervention.

Automatic reactions make enterprise applications faster, smarter, and more reliable.

---

# Reflective Questions

## 1. Why do systems need triggers?

Triggers help systems automatically respond to data changes without manual effort. They improve efficiency, accuracy, and real-time processing.

---

## 2. Difference between polling and event-driven systems?

| Polling System                  | Event-Driven System              |
| ------------------------------- | -------------------------------- |
| Continuously checks for changes | Reacts only when an event occurs |
| Wastes resources                | More efficient                   |
| Slower response                 | Faster response                  |
| Example: Refreshing repeatedly  | Example: Trigger execution       |

---

## 3. Why are database queries important?

Database queries help retrieve specific information quickly from large datasets. Without queries, finding required data would be slow and difficult.

---

## 4. When should Flows be preferred over Triggers?

Flows should be preferred when:

* Automation is simple
* No coding is needed
* Admins manage the process
* Quick configuration is required

Example:
Sending approval notifications or updating simple fields.

---

## 5. What problems happen if automation logic becomes too complex?

Complex automation can cause:

* Slow system performance
* Difficult debugging
* Unexpected errors
* Maintenance challenges
* Automation conflicts

---

## 6. Why should developers think carefully before automating actions?

Poor automation can create incorrect updates, duplicate actions, or performance issues. Developers must ensure automation is accurate, efficient, and necessary before implementing it.

