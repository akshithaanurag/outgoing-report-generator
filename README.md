# iaeste-report-automation-

The **Outgoing Exchange Coordinator** is a browser-based task management and reporting system designed to help student exchange program coordinators efficiently handle their daily activities. With no server or database dependency, this tool works entirely offline using `localStorage`, making it simple, secure, and highly portable.

---

## 🎯 Purpose

Managing exchange-related tasks like nominations, acceptances, and cancellations across different categories (like internships or reserved offers) can be chaotic. This application:

- Keeps track of every coordinator's actions
- Simplifies reporting with one-click report generation
- Provides filtered statistics per category
- Ensures quick data entry with a clean UI

---

## 🚀 Features Overview

| Feature                          | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| 🧑‍💼 Login System                 | Simple login using coordinator name (no passwords)                         |
| 📝 Task Management              | Add tasks with categories, types, candidate names, and action types        |
| 📋 Task Display                 | Tasks are shown filtered by the logged-in coordinator                      |
| 📊 Report Generation            | One-click Weekly, 15-Day, and Monthly reports                              |
| 📈 Statistics View              | View structured stats for all categories and offer types                   |
| 🗑️ Admin Delete                 | Clear all data with one click (with confirmation)                          |
| 💾 Local Storage                | Tasks persist between sessions with `localStorage`                         |

---

## 🖥️ How It Works

Once a coordinator logs in, they can:

1. **Add new tasks** like "Nomination", "Rejection", or custom actions.
2. **Select offer categories**:  
   - Global Internship (e.g., COBE, FCFS)  
   - Exchange Offers (e.g., Open, April, Winter, Autumn)  
   - Reserved Offers (no subtype)
3. View a **task list**, filtered only to their entries.
4. Generate reports:
   - **Weekly Report** (last Sunday to Saturday)
   - **15-Day Summary**
   - **Monthly Report** (1st to current day)
5. View **statistics** per offer and action (Nominated, Rejected, etc.)
6. Use the admin option to **delete all tasks** when needed.

---

## 🧠 Task Object Structure

Each task is stored in this format inside the browser:

```json
{
  "coordinator": "Alice",
  "datetime": "2025-06-06T13:30:00.000Z",
  "offerCategory": "Global Internship",
  "offerType": "COBE",
  "taskAction": "Nomination",
  "offerNumber": "12345",
  "candidateName": "John Doe"
}


📁 OutgoingExchangeCoordinator/
├── index.html     # Main HTML structure and UI
├── styles.css     # All styles: layout, responsive design, dark mode
├── script.js      # Full logic: login, task handling, reporting
└── README.md      # Project documentation


![Login Page](Screenshot-login)
![Task Entry](Screenshot-task-entry)
![Report Example](Screenshot-report)
