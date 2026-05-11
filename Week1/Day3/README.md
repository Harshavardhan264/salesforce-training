# 🎓 College Management System – Salesforce Data Model

---

# 📌 1. Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|------|----------|----------|
| **App** | Collection of tabs, objects, and features | College Management System App |
| **Object** | Database table that stores data | Student, Faculty |
| **Record** | Single entry inside an object | Harsha student record |
| **Field** | Individual data stored in a record | Name, Email, Age |

---

# 📘 2. Standard vs Custom Objects

| Standard Objects | Custom Objects |
|------------------|----------------|
| Already provided by Salesforce | Created by users |
| Examples: Account, Contact, Lead | Examples: Student, Faculty |
| Used for common CRM tasks | Used for project-specific needs |
| Cannot be deleted easily | Fully customizable |

✅ In this project, we created custom objects:

- Student  
- Faculty  
- Course  
- Department  

---

# 🏗️ 3. College Data Model

## 📦 Objects Created

- 🎓 Student  
- 👨‍🏫 Faculty  
- 📚 Course  
- 🏢 Department  

---

## 🔗 Relationships

| Parent Object | Child Object | Relationship Type |
|----------------|--------------|-------------------|
| Department | Student | Lookup |
| Department | Faculty | Lookup |
| Department | Course | Lookup |
| Faculty | Course | Lookup |

---

## 📊 Data Model Diagram

```text
Department
   ├── Students
   ├── Faculty
   └── Courses

Faculty
   └── Courses
```

---

# 🧮 4. Formula Fields

## ✅ Formula Field 1 — Percentage

### Formula

```text
(Obtained_Marks__c / Total_Marks__c) * 100
```

### Why use Formula Field?

- Automatically calculates student percentage  
- Reduces manual calculation errors  
- Saves time  

---

## ✅ Formula Field 2 — Remaining Seats

### Formula

```text
Total_Seats__c - Filled_Seats__c
```

### Why use Formula Field?

- Shows available seats instantly  
- Prevents overbooking  
- Improves course management  

---

## ✅ Formula Field 3 — Full Name

### Formula

```text
First_Name__c & " " & Last_Name__c
```

### Why use Formula Field?

- Combines names automatically  
- Keeps formatting consistent  
- Avoids duplicate typing  

---

# 🔒 5. Validation Rules

## ✅ Rule 1 — Email Cannot Be Empty

### Formula

```text
ISBLANK(Email__c)
```

### Purpose

Prevents saving student records without email.

---

## ✅ Rule 2 — Age Cannot Be Negative

### Formula

```text
Age__c < 0
```

### Purpose

Prevents invalid age values.

---

## ✅ Rule 3 — Filled Seats Cannot Exceed Total Seats

### Formula

```text
Filled_Seats__c > Total_Seats__c
```

### Purpose

Prevents over-enrollment in courses.

---

# 💡 6. Reflection — Why Structured Enterprise Data Matters

Structured enterprise data helps organizations store and manage information in a clear and organized way. Systems like Salesforce connect related data using objects and relationships, making it easier to search, analyze, and generate reports.

Structured data reduces duplication, improves accuracy, increases security, and supports automation. Unlike random spreadsheets, enterprise systems provide better collaboration, faster decision-making, and scalable business operations.

---

# 🚀 Technologies Used

- Salesforce Trailhead  
- Custom Objects  
- Lookup Relationships  
- Formula Fields  
- Validation Rules  
- Lightning App  

---

# 📱 Final Output

✅ College Management System App created successfully with:

- Custom Objects  
- Relationships  
- Formula Fields  
- Validation Rules  
- Lightning Navigation App  
