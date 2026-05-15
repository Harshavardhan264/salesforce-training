# Day 4 - Flow Builder 🚀

## What is Flow Builder?

Flow Builder is a Salesforce automation tool used to automate business processes without coding.  
It helps users create workflows, send emails, update records, display screens, and automate repetitive tasks using a visual interface.

---

# Types of Flows

## 1. Screen Flow
Screen Flow is used to create interactive forms or screens for users.  
It collects input from users and performs actions based on the entered data.

### Example:
- Student Registration Form
- Fee Payment Form
- Course Enrollment Form

---

## 2. Record-Triggered Flow
Record-Triggered Flow runs automatically when a record is created, updated, or deleted.

### Example:
- Send email after student registration
- Update remaining seats automatically
- Generate student ID automatically

---

# My Automation Ideas 💡

## 1. Auto Email After Student Registration
When a student registers, Salesforce automatically sends a welcome email.

## 2. Auto Update Remaining Seats
Available seats decrease automatically when a student enrolls in a course.

## 3. Notify Faculty When Course is Full
Faculty receives notification when all seats are filled.

## 4. Generate Student ID Automatically
Salesforce automatically creates a unique student ID.

## 5. Send Reminder Before Fee Deadline
Students receive automatic reminders before fee due dates.

---

# My Flow Diagram 🔄

## Auto Email After Student Registration

```text
[Student Record Created]
            ↓
 [Record-Triggered Flow Starts]
            ↓
      [Send Email Action]
            ↓
 [Welcome Email Sent]
```



---

# Manual vs Automated Process

## Process: Fee Payment Reminder

### Manual Process
- Staff manually checks fee records.
- Reminder emails or calls are sent one by one.
- High chance of missing students.

### Problems in Manual Process
- Time-consuming
- Human errors
- Delayed reminders
- More staff effort required

### Automated Process Using Salesforce
- Salesforce automatically tracks fee due dates.
- Reminder emails are sent automatically.
- Faster and more accurate communication.
- Reduces manual work and saves time.

---

# Reflection ✨

## Why automation matters in enterprise systems

Automation helps companies improve efficiency, accuracy, and productivity.  
It reduces repetitive manual work, saves time, minimizes human errors, and improves communication.  
Enterprise systems like Salesforce use automation to handle large business processes quickly and reliably.  
Automation also helps employees focus on important and creative tasks instead of repetitive operations.

---

# Tools Used 🛠️
- Salesforce Trailhead Playground
- Flow Builder
- Custom Objects
- Record-Triggered Flows

---

# Outcome 🎯
Learned how to use Salesforce Flow Builder to automate business processes in a College Management System.
