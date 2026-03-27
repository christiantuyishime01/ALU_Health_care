# 🏥 ALU Healthcare Dashboard

A full-featured campus health and academic management web application built for the African Leadership University. It includes student authentication, a health service request form, hydration and sports tracking, course management, grades, inbox, and a personal profile — all running entirely in the browser with no backend required.

---

## 🌐 Live Demo

> **https://github.com/christiantuyishime01/ALU_Health_care.git**

---

## 📁 Project Files

Your repository must contain exactly these three files:

```
alu-healthcare/
├── index.html       ← Login & registration page (entry point)
├── dashboard.html   ← Main application dashboard
└── README.md        ← This file
```

---

## ✨ Features

- 🔐 **Authentication** — User registration and login with data stored in the browser
- 👤 **User Profiles** — View and edit personal information saved from registration
- 🏥 **Health Service Request** — 4-step form to request medical, mental health, physiotherapy, dental, and other campus services
- 💧 **Hydration Tracker** — Log daily water intake with reminders
- 🏃 **Sports & Activity Scheduler** — Check off daily fitness activities
- 📚 **Courses** — View enrolled courses and progress
- 📝 **Assignments** — Track upcoming and overdue work
- 📅 **Calendar** — Monthly event overview
- 📊 **Grades** — GPA and course grade summaries
- 💬 **Discussions & Inbox** — Forum threads and messages
- 📁 **Files** — Document management
- 🌿 **Health Hub** — Wellness tracking with weekly summary

---

## 🔑 How to Log In

When you open the live URL you will land on the login page. You have two options:

### Option A — Use a Demo Account (Fastest)

Click any of the four demo buttons on the login page:

| Button | Email | Password | Role |
|--------|-------|----------|------|
| Amara K. | student@alu.edu | demo1234 | Student |
| James M. | trainer@alu.edu | demo1234 | Trainer |
| Dr. Reeves | health@alu.edu | demo1234 | Clinician |
| Admin | admin@alu.edu | demo1234 | Administrator |

The email and password fill in automatically — just click **Sign In**.

### Option B — Create Your Own Account

1. Click the **Create Account** tab on the login page
2. Enter your **first name** and **last name**
3. Enter your **email address** and a **password** (minimum 6 characters)
4. Select your **role** — Student, Trainer, or Clinician
5. Click **Create Account**

Your account is saved permanently in the browser's local storage. It will still be there the next time you visit the site on the same device and browser.

---

## 🗺️ Navigating the Dashboard

After logging in you will see the main dashboard. Use the left sidebar to navigate between sections:

| Section | Description |
|---------|-------------|
| ⊞ Dashboard | Overview with stats, upcoming assignments, announcements, and wellness cards |
| 📚 Courses | All enrolled courses with progress bars |
| 📝 Assignments | Upcoming, due soon, and overdue assignments |
| 📅 Calendar | Monthly calendar with event indicators |
| 📊 Grades | GPA tracker and course-by-course grades |
| 💬 Discussions | Community forum threads |
| 📥 Inbox | Messages from instructors and staff |
| 📁 Files | Uploaded course documents |
| 💪 Health Hub | Water tracker, sports schedule, and weekly wellness summary |
| 🏥 Health Request | Submit a campus health service request |
| 👤 My Profile | View and edit your account information |
| 🚪 Sign Out | Log out and return to the login page |

---

## 🏥 Using the Health Service Request

The Health Service Request is a 4-step form to book a medical appointment on campus.

**Step 1 — Choose a Service Type**
Select from 9 service categories including General Consultation, Mental Health, Physiotherapy, Nutrition, Dental, Eye Care, Vaccination, Lab Tests, and Urgent Care. Then set your priority level (Low, Medium, or High).

**Step 2 — Enter Your Details**
Fill in your name, student ID, email, phone, date of birth, symptoms, allergies, and current medications. Your name and email are pre-filled from your profile automatically.

**Step 3 — Schedule Your Appointment**
Pick a preferred date, choose between In-Person, Virtual, or Home Visit, and select an available time slot. Slots already taken by other students are shown in grey. You can also request a specific clinician.

**Step 4 — Review and Submit**
Check all your information before submitting. After submission you receive a unique reference code (e.g. `ALU-382910`) and the request is saved to your browser storage. You can view all your past requests by clicking **My Requests** tab.

---

## 💾 How Data is Stored

This project runs entirely in the browser — there is no server or database in the cloud. Here is where each type of data is saved:

| Data | Storage | When it clears |
|------|---------|----------------|
| Registered user accounts | `localStorage` | Never (stays until browser data is cleared) |
| Health service requests | `localStorage` | Never (stays until browser data is cleared) |
| Login session | `sessionStorage` | When the browser tab is closed |
| Water and sports tracking | In memory | When the page is refreshed |

> **Important:** Because data is stored in the browser, each person's data is private to their own device and browser. Data does not sync between devices.

---


## 🏫 About

Built for the **African Leadership University (ALU)** Healthcare Division as a student wellness and academic management platform.



## 📄 License

This project is open source and free to use for educational purposes.
