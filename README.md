# ☁️ SkillSwap Cloud

### Cloud-Based Student Skill Exchange Platform

**Share What You Know. Learn What You Need.**

SkillSwap Cloud is a cloud-based web application that allows college students to exchange knowledge and skills with other students.

Students can list the skills they can teach, specify the skills they want to learn, discover other students and find suitable skill-exchange partners.

---

## 📌 Project Overview

Students have different technical and non-technical skills.

For example:

* Student A knows Python but wants to learn UI/UX Design.
* Student B knows UI/UX Design but wants to learn Python.

SkillSwap Cloud identifies this as a **mutual skill match** and allows the students to send an exchange request.

The goal is to create a collaborative learning environment where students can learn from each other.

---

## 🎯 Objectives

* Create a platform for student-to-student skill exchange.
* Allow students to create skill profiles.
* Help students discover new skills.
* Find suitable skill-exchange partners.
* Provide exchange request management.
* Provide student messaging.
* Demonstrate the use of cloud computing technologies.
* Store application data securely in a cloud database.

---

## ☁️ Cloud Computing Concept

The project uses cloud services for the major application components.

| Component         | Technology            |
| ----------------- | --------------------- |
| Frontend          | HTML, CSS, JavaScript |
| Cloud Database    | Supabase PostgreSQL   |
| Authentication    | Supabase Auth         |
| Cloud Storage     | Supabase Storage      |
| Realtime Features | Supabase Realtime     |
| Hosting           | GitHub Pages          |

Supabase provides PostgreSQL, authentication and other cloud services that can be integrated into a web application.

The static frontend can be deployed using GitHub Pages.

---

## ✨ Features

### 👤 Student Features

* Student registration
* Student login
* Student profile
* Profile editing
* Add skills
* Remove skills
* Skill categories
* Skill levels
* Search skills
* Explore students
* Find skill matches
* Exchange requests
* Active exchanges
* Student messaging
* Notifications

### 🔄 Skill Matching

The system compares:

**Skills Offered ↔ Skills Wanted**

and identifies suitable students.

Example:

```text
Student A
Offers: Python
Wants: UI/UX

Student B
Offers: UI/UX
Wants: Python

Result:
Mutual Skill Match
Compatibility: 100%
```

---

## 🏗️ System Architecture

```text
                Student
                   │
                   ▼
          ┌─────────────────┐
          │ SkillSwap Cloud │
          │ HTML/CSS/JS     │
          └────────┬────────┘
                   │
                   ▼
          ┌─────────────────┐
          │    Supabase     │
          │     Cloud       │
          └────────┬────────┘
                   │
       ┌───────────┼───────────┐
       ▼           ▼           ▼
   PostgreSQL     Auth       Storage
   Database      Login       Images
       │
       ▼
    Realtime
 Messages/Updates
```

---

## 🛠️ Technologies Used

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend / Cloud

* Supabase
* PostgreSQL
* Supabase Authentication
* Supabase Storage
* Supabase Realtime

### Deployment

* GitHub
* GitHub Pages

---

## 📂 Project Structure

```text
skillswap-cloud/
│
├── index.html
├── login.html
├── register.html
├── dashboard.html
├── profile.html
├── skills.html
├── explore.html
├── matches.html
├── requests.html
├── exchange.html
├── messages.html
├── notifications.html
├── admin.html
│
├── css/
│   ├── style.css
│   ├── dashboard.css
│   └── responsive.css
│
├── js/
│   ├── supabase.js
│   ├── auth.js
│   ├── profile.js
│   ├── skills.js
│   ├── explore.js
│   ├── matches.js
│   ├── requests.js
│   ├── exchange.js
│   ├── messages.js
│   └── admin.js
│
├── assets/
│   ├── images/
│   └── icons/
│
├── database/
│   └── schema.sql
│
└── README.md
```

---

## 🗄️ Database Tables

The project uses the following tables:

### profiles

Stores student profile information.

### skills

Stores available skills and categories.

### student_skills

Connects students with their offered and wanted skills.

### exchange_requests

Stores skill-exchange requests.

### exchanges

Stores accepted skill exchanges.

### messages

Stores student messages.

### notifications

Stores system notifications.

---

## 🔐 Security

The project uses Supabase Authentication and Row Level Security.

Security rules should ensure that:

* Students can update their own profiles.
* Students can manage their own skills.
* Students cannot modify another student's profile.
* Students can manage exchange requests involving them.
* Students can access their own messages.
* Admin functionality is restricted to administrators.

Never expose a Supabase service-role key in frontend code.

---

## 🚀 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/skillswap-cloud.git
```

### 2. Open the project

Open the folder in VS Code.

### 3. Create a Supabase project

Create a Supabase project and obtain the project URL and public client key.

### 4. Create the database

Open the Supabase SQL Editor.

Run:

```text
database/schema.sql
```

This creates the required tables and security policies.

### 5. Configure Supabase

Open:

```text
js/supabase.js
```

Add your Supabase project URL and public client key.

Do not add the Supabase service-role key to frontend code.

### 6. Run the website

Use VS Code Live Server or another local static server.

Open:

```text
index.html
```

---

## 🌐 Deployment

The frontend can be hosted using GitHub Pages because it consists of static HTML, CSS and JavaScript files.

Basic deployment:

```text
1. Create GitHub repository
2. Upload project files
3. Open repository Settings
4. Select Pages
5. Select the main branch
6. Save
7. Open the generated GitHub Pages URL
```

Supabase continues to provide the cloud database and authentication services.

---

## 🔄 Application Workflow

```text
Register
   ↓
Create Profile
   ↓
Add Offered Skills
   ↓
Add Wanted Skills
   ↓
Explore Students
   ↓
Find Skill Match
   ↓
Send Exchange Request
   ↓
Accept Request
   ↓
Active Exchange
   ↓
Learn & Share
   ↓
Complete Exchange
```

---

## 📊 Example

### Student A

```text
Offers:
Python

Wants:
UI/UX Design
```

### Student B

```text
Offers:
UI/UX Design

Wants:
Python
```

### SkillSwap Result

```text
🎯 Mutual Skill Match

Student A ↔ Student B

You Teach:
Python

You Learn:
UI/UX Design

Compatibility:
100%

Status:
Available
```

---

## 🌟 Advantages

* Encourages peer-to-peer learning.
* Helps students discover hidden talents.
* Reduces dependence on traditional learning methods.
* Provides a centralized skill-sharing platform.
* Accessible from different devices.
* Uses cloud-based data storage.
* Can be scaled for multiple colleges.
* Provides a practical demonstration of cloud computing.

---

## 🔮 Future Enhancements

Future versions could include:

* AI-based skill recommendations
* College-wise communities
* Skill certificates
* Student ratings and reviews
* Calendar integration
* Video-learning integration
* Advanced analytics
* Mobile application
* Multi-college deployment

---

## 🎓 Academic Project

**Project:** SkillSwap Cloud
**Domain:** Cloud Computing
**Type:** Web Application
**Target Users:** College Students

---

## 📜 License

This project is created for educational and academic purposes.
