# Student Management System (SMS) Capstone Project

Welcome to the Student Management System (SMS) Capstone Project. This project is part of the Ideas Programme at Base University for software engineering students. This README file provides a step-by-step guide on setting up and understanding the core functionalities of the system.

## Overview

The Student Management System is a web application designed to manage student records. It includes features for adding, updating, and viewing student information. The application also allows for the deletion of student records.

## Table of Contents

1. [Project Structure](#project-structure)
2. [Setup Instructions](#setup-instructions)
3. [Usage](#usage)
4. [Features](#features)
5. [Technologies Used](#technologies-used)
6. [Known Issues](#known-issues)
7. [License](#license)

## Project Structure

The project is organized as follows:

- `students/`
  - `templates/`
    - `students/`
      - `base.html` – The base template that includes the common layout for all pages.
      - `add_student.html` – Template for adding a new student.
      - `update_student.html` – Template for updating existing student records.
      - `all_students.html` – Template for displaying all student records.

## Setup Instructions

Follow these steps to set up the Student Management System on your local machine:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Gifftybabe/Student-Management-System.git
   ```

2. **Navigate to the Project Directory**
   ```bash
   cd student-management-system
   ```

3. **Set Up a Virtual Environment**
   - **For Windows:**
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - **For macOS/Linux:**
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

4. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run Database Migrations**
   ```bash
   python manage.py migrate
   ```

6. **Create a Superuser (Optional)**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the Development Server**
   ```bash
   python manage.py runserver
   ```
   Open `http://127.0.0.1:8000` in your web browser to view the application.

## Usage

### Adding a Student
- Navigate to the "Add Student" page via the main navigation menu.
- Fill out the form with the student's information and submit.

### Updating a Student
- Navigate to the "All Students" page to view the list of students.
- Click the "Edit" button next to the student record you wish to update.
- Modify the information and submit the form.

### Viewing Students
- Navigate to the "All Students" page to view a table of all student records.
- Click the "View" button next to any student record to see detailed information.

### Deleting a Student
- Navigate to the "All Students" page.
- Click the "Delete" button next to the student record you wish to remove.
- Confirm the deletion in the modal that appears.

## Features

- **Student Registration:** Allows adding new students with details such as student number, name, email, field of study, and GPA.
- **Update Records:** Enables updating existing student information.
- **View Records:** Provides a detailed view of individual student information.
- **Delete Records:** Allows removing student records from the system.
- **Responsive Design:** The application is designed to be responsive and user-friendly on different devices.

## Technologies Used

- **Frontend:**
  - HTML
  - CSS (Bootstrap)
  - JavaScript (FontAwesome)

- **Backend:**
  - Django (Python)
  - SQLite (Database)

## Known Issues

- **Form Validation:** Ensure all fields are properly validated before submitting. There may be some edge cases where validation fails.
- **User Interface:** The user interface may not be fully optimized for all screen sizes. Future updates may include more responsive design improvements.

