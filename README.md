# Interview Management System
The Interview Management System is designed to streamline hiring by organizing job descriptions, candidate data, interview schedules, and interviewer information in a single application. This app allows seamless tracking and management of interviews, candidate status, and interviewer details.

# Table of Contents
Overview
Features
Setup
Usage
Kanban Board
Additional Tasks

## Overview
The Interview Management System includes the following components:
Job Description (JD): A web page displaying job details, such as the company name, location, and role. Candidate Data: A DocType to store and filter candidate information based on experience and applied role. Interview Schedule: A schedule with a defined workflow to track interview progress and outcomes. Interviewer Information: A DocType to manage interviewer details, with data import functionality.

## Features
Web Page - Job Description: Displays job details, company name, location, role, work type, and available openings. Includes an "Apply" button that opens an application form for candidates. Doctype: Candidate’s Data: Tracks candidate's name, experience, skills, and applied role. Filter options are available for experienced and applied roles. Doctype: Interviewer Information: Stores information for interviewers, including name, contact, position, department, and address. Data can be imported via a Google Sheet CSV (e.g., entries for users Manisha, and Swati). Doctype: Interview Schedule: Manages the interview schedule, linking candidate names and interviewer names, as well as details like the role applied for, interview date, and current status. Status options are color-coded: "Hired" (green), "Rejected" (red), and "In Progress" (yellow). Naming rule format: cdn-role-intName (e.g., "cdn-frontend-Manisha").

## Setup
Clone the Repository: git clone https://github.com/Kusum23-sinha/Interview-Management-system. git cd InterviewManagementSystem Install Dependencies: Follow the development framework's instructions to install any required dependencies.
Database Setup: Run migrations to initialize the required database tables: bench migrate Import Interviewer Data: Use Google Sheet CSV import to upload interviewer data for initial setup.
Start the Server: bench start

## Usage
Web Page (Job Description):
View job descriptions with details like company name, role, location, and work type (Remote, Office). Click "Apply" to open the application form for candidates. Candidate Data:
Add or edit candidate records with Name, Experience, Skills, and Applied Role fields. Use filters to view candidates by experience or applied role. Interview Schedule:
Create new interview schedules by linking candidate and interviewer data. Assign a date and role to each interview, and update the status as "Hired," "Rejected," or "In Progress." Interviewer Information:
Add or import interviewer records, including details like name, position, contact, department, and address.

## Kanban Board (ToDo App)
The system includes a Kanban board feature for managing interview tasks:
To Do: Schedule interviews. In Progress: Interviews in progress. Completed: Interviews with a finalized outcome.

## Additional Tasks
Date Validation: Ensures dates are valid and consistent across the application. Custom Buttons: "Hire" and "Reject" buttons were added for easier status management. Delete Message Alert: Alerts users before deleting a record. Welcome Notification: Displays a welcome message on the candidate page. Submittable Data: Once a candidate is hired, the data becomes submittable. Remove Email Login: Email login functionality is disabled.

 InterviewManagement/README.md at main · Kusum23-sinha/ Interview-Management-system



