DoubtShare
DoubtShare is an interactive real-time doubt solving platform designed to assist students with their academic queries.

Table of Contents
Introduction
Features
Tech Stack
Folder Structure
Getting Started
API Endpoints
Usage
Contributing
License
Introduction
DoubtShare is a platform where students can get real-time assistance with their academic doubts. Tutors are available to help students in various subjects, making the learning process more interactive and personalized.

Features
User Authentication:

Users can register and log in as either students or tutors.
Token-based authentication ensures secure access.
Real-Time Doubt Resolution:

Students can create doubt requests specifying the subject and their question.
Online tutors matching the subject, language, and class grade are notified in real-time.
The first tutor who accepts the request engages in a chat consultation with the student.
Doubt History:

Students can view their doubt history, including past doubts and their resolutions.
Database Structure:

Well-defined database structure with tables for users, tutors, doubt requests, and tutor availability.
Scheduled Tasks:

Polling function updates tutors' availability every 3 seconds.
CRON job runs every second to count real-time available tutors.
Tech Stack
React (Frontend)
Node.js (Backend)
Postgres (Database)
Folder Structure
The project is organized into folders for frontend, backend, database, and scheduled tasks. The structure promotes modularity and separation of concerns.

For more details, refer to the Folder Structure section in this README.

Getting Started
To set up the DoubtShare app on your local machine, follow the steps below:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/doubtshare.git
Navigate to the project directory:

bash
Copy code
cd doubtshare
Install dependencies for both the frontend and backend:

bash
Copy code
cd client && npm install
cd ../server && npm install
Set up the database and run migrations:

bash
Copy code
cd ../database
# Run your database migration scripts here
Start the development server for both frontend and backend:

bash
Copy code
cd ../client && npm start
cd ../server && npm start
Access the DoubtShare app in your browser at http://localhost:3000.

API Endpoints
Authentication:

/api/register (POST): User registration.
/api/login (POST): User login.
Doubt Handling:

/api/doubt/create (POST): Create a new doubt request.
/api/doubt/history/:userId (GET): Get doubt history for a specific student.
For more details, refer to the API Endpoints section in this README.

Usage
...

Contributing
...

License
This project is licensed under the MIT License.# DoubtShare
