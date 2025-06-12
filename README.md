Outgoing-Report-Generator

A browser-based task and reporting system for IAESTE Outgoing Exchange Coordinators.
This lightweight tool helps coordinators manage actions like nominations, rejections, and acceptances across various offer categories—all offline using localStorage.

Purpose
   Coordinating outgoing exchange tasks involves multiple offer categories and types. This tool simplifies the workflow by:
   Allowing fast task entry
   Filtering tasks per coordinator
   Generating clean reports in a click
   Displaying statistics by category and action
   Working completely offline (no backend)

Features
   Coordinator login (no password)
   Add tasks with offer details and candidate info
   View tasks filtered by logged-in user
   Generate:
      Weekly reports (last 7 days)
      15-Day reports
      Monthly reports (from 1st of month)
   View action-based and category-based statistics
   Admin option to clear all data
   All data stored locally via localStorage

How It Works
   Login with your coordinator name
   Add new tasks with:
      Offer Category (Global Internship, Exchange, Reserved)
      Offer Type (COBE, FCFS, etc.)
      Action Type (Nomination, Rejection, etc.)
      Candidate Name and Offer Number
   View your task list
   Generate reports instantly
   Review statistics
   Clear all entries (admin only)

Project Structure
   OutgoingExchangeCoordinator/
├── index.html             # Main HTML and UI structure
├── styles.css             # Styling for layout, dark mode, responsiveness
├── script.js              # All logic: login, task handling, reports, stats
├── Screenshot-login.png   # Screenshot of login page
├── Screenshot-task-entry.png  # Screenshot of task entry form
├── Screenshot-report.png      # Screenshot of report view
└── README.md              # Project documentation

Screenshot Previews
![Screenshot-login](https://github.com/user-attachments/assets/ea11e947-554b-4751-822c-12cdc3627d3b)

![Screenshot-task-entry](https://github.com/user-attachments/assets/18084c05-c98d-40e6-ab05-fa0a3776d3fd)

![Screenshot-report](https://github.com/user-attachments/assets/a0e68625-27bd-4c3f-8f7b-101cf24d9b46)


Data Format
Tasks are stored in the following format:
{
  "coordinator": "Alice",
  "datetime": "2025-06-06T13:30:00.000Z",
  "offerCategory": "Global Internship",
  "offerType": "COBE",
  "taskAction": "Nomination",
  "offerNumber": "12345",
  "candidateName": "John Doe"
}

License
This project is licensed under the MIT License

Author
   Akshitha Anurag
   Live Demo: https://akshithaanurag.github.io/outgoing-report-generator/
