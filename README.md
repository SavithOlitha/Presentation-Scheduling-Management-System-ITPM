# 📅 Smart Presentation Scheduler System

This is a university-level group project developed using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The system is designed to simplify and automate the process of scheduling student presentations by managing students, examiners, venues, groups, modules, and rescheduling requests. It includes a unique smart scheduling suggestion feature to avoid clashes and optimize availability.

---

## 📌 Table of Contents

- [Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [Core Features](#core-features)
- [Module Breakdown](#module-breakdown)
- [Smart Suggest Function](#smart-suggest-function)
- [Report Generation](#report-generation)
- [System Workflow](#system-workflow)
- [Setup Instructions](#setup-instructions)
- [Contributors](#contributors)
- [License](#license)

---

## 🔍 Project Overview

Scheduling academic presentations involving students, examiners, and venues is often time-consuming and error-prone. Our system addresses this problem by providing a centralized web application where administrators can:

- Add and manage students, examiners, and modules
- Organize students into groups
- Allocate venues and timetables
- Create and reschedule presentations
- Approve or reject rescheduling requests
- Generate reports for administrative use

The system includes a **Smart Suggest Feature** that automatically checks availability and suggests optimal time slots and venues.

---

## 🧰 Tech Stack

| Layer       | Technology         |
|-------------|--------------------|
| Frontend    | React.js           |
| Backend     | Node.js, Express.js|
| Database    | MongoDB            |
| Styling     | Tailwind CSS / Bootstrap |
| Auth        | JWT (JSON Web Token) |
| Deployment  | (Optional: Heroku, Vercel, or Netlify) |

---

## 💡 Core Features

- CRUD operations for:
  - Students
  - Examiners
  - Groups
  - Venues
  - Modules
  - Timetables
  - Presentations
  - Rescheduling requests

- **Smart Suggest System** to automate scheduling and conflict detection
- **Report generation** for all entities
- **Search and filter** functionalities
- **Admin approval system** for rescheduling
- **User notifications** for presentation status changes

---

## 📚 Module Breakdown

### 👩‍🎓 Nuwangi – *Student & Group Management*
- Add/view/update/delete student records
- Manage group creation
- Add students to groups through search
- Generate reports on students and group allocations

### 👩‍🏫 Amanda – *Examiner, Venue, and Module Management*
- Examiner CRUD with specialization and availability
- Venue management (CRUD) with capacity and availability
- Module management based on faculty and degree type
- Generate venue/module assignment reports

### 👨‍💻 Olitha – *Presentation Scheduling*
- Manually schedule presentations (CRUD)
- Smart Suggest to automatically select time slots and venues
- Modify existing presentation details
- Handle scheduling conflicts and dependencies
- Generate final presentation timetables

### 👩‍💼 Aseni – *Rescheduling & Timetable Management*
- View, approve, or reject rescheduling requests
- Use smart suggest to validate requested time
- Track and delete old rescheduling requests
- Add and manage group-specific timetables
- Report generation for rescheduled requests

---

## 🧠 Smart Suggest Function

A key feature in this system is the **Smart Suggest** algorithm, which uses database queries and availability checks to:

- Recommend time slots for presentations
- Avoid clashes in examiner/student schedules
- Ensure venue availability and capacity
- Provide dynamic suggestions when rescheduling

This function is used in both **initial scheduling** and **rescheduling** scenarios to streamline the process.

---

## 📈 Report Generation

All modules support automatic report generation. These reports are useful for academic tracking and admin audits.

| Module               | Reports Generated                   |
|----------------------|-------------------------------------|
| Student Management   | Student List, Faculty-wise Report   |
| Group Management     | Group Allocations                   |
| Examiner Management  | Examiner Directory                  |
| Presentation         | Timetable Report                    |
| Rescheduling         | Rejected/Approved Requests Log      |
| Module Management    | Module Assignments by Degree        |

---

## 🔄 System Workflow

1. **Admin adds students, examiners, venues, and modules**
2. **Groups are created with assigned students**
3. **Presentations are scheduled manually or via Smart Suggest**
4. **Examiners can request rescheduling due to conflict**
5. **Admin approves/rejects requests with Smart Suggest assistance**
6. **All updates are reflected on both student and examiner dashboards**

---

## 🛠️ Setup Instructions

### 🔗 Clone Repository
```bash
git clone https://github.com/your-repo/presentation-scheduler.git
