# Day 5 - Apex Introduction ⚡

## What is Apex?

Apex is a programming language developed by Salesforce.  
It is used to add custom business logic and automation in Salesforce applications.

Apex is similar to Java and runs on the Salesforce platform.  
It helps developers create advanced features that cannot be achieved using only Flow or configuration tools.

---

# Difference Between Flow and Apex

| Flow | Apex |
|---|---|
| No-code/low-code automation tool | Programming language |
| Easy to build using drag-and-drop | Requires coding knowledge |
| Best for simple automation | Best for complex logic |
| Faster development | More customization and control |
| Used by admins | Used by developers |

---

# Difference Between Configuration and Coding

| Configuration | Coding |
|---|---|
| Uses clicks, settings, and tools | Uses programming languages |
| No programming required | Programming knowledge required |
| Faster and easier | More flexible and powerful |
| Limited customization | Advanced customization possible |
| Example: Flow Builder | Example: Apex Classes |

---

# Real Examples Where Apex Is Needed 💡

## 1. Complex Fee Calculation
Calculate scholarship discounts, late fees, and taxes dynamically based on student categories.

## 2. Bulk Student Data Processing
Process thousands of student records efficiently using batch operations.

## 3. Third-Party Integration
Connect the College Management System with external payment gateways or university portals using APIs.

---

# Integrated System Design 🏫

## CRM
Salesforce CRM is used to manage student data, courses, faculty details, fees, and communication.

---

# Objects

## Custom Objects Used
- Student
- Course
- Enrollment
- Faculty
- Fee

---

# Relationships

| Parent Object | Child Object | Relationship |
|---|---|---|
| Student | Enrollment | Lookup |
| Course | Enrollment | Lookup |
| Faculty | Course | Lookup |

---

# Validation

Validation Rules are used to maintain accurate data.

### Examples:
- Student email must be valid.
- Fee amount cannot be negative.
- Course seats cannot go below zero.

---

# Flow Automation

## Examples of Flows
- Auto email after student registration
- Auto update remaining seats
- Fee reminder notifications
- Generate student ID automatically

---

# Apex Usage

Apex is used for:
- Complex calculations
- API integrations
- Advanced business logic
- Batch processing
- Custom triggers

---

# Pseudocode Examples 🧠

## 1. Auto Reduce Course Seats

```text
IF student enrolls in course
THEN reduce available seats by 1
UPDATE course record
```

---

## 2. Send Fee Reminder

```text
IF fee due date is near
THEN send reminder email to student
```

---

## 3. Generate Student ID

```text
WHEN new student record is created
GENERATE unique student ID
SAVE student record
```

---

# Reflection ✨

## Why enterprise systems eventually need programming

Enterprise systems initially use configuration tools because they are fast and easy.  
However, as business requirements become more complex, programming becomes necessary.

Large organizations need:
- Advanced automation
- Complex calculations
- External system integrations
- High-performance processing
- Custom security and validation

Programming languages like Apex provide flexibility and scalability that configuration tools alone cannot achieve.  
Therefore, enterprise systems eventually require coding to handle real-world business challenges efficiently.

---

# Tools Used 🛠️
- Salesforce CRM
- Flow Builder
- Apex
- Validation Rules
- Custom Objects

---

# Outcome 🎯
Learned the basics of Apex and understood how coding and automation work together in enterprise Salesforce applications.
