# LearnHub – Learning Management System

A Django-based LMS starter project with student/instructor roles, course creation, lessons, enrollment, lesson completion tracking, and a responsive interface.

## Features
- Register, login, and logout
- Student and instructor accounts
- Instructor course creation and lesson management
- Course catalogue and course details
- Student course enrollment
- Lesson viewing and completion tracking
- Student dashboard with enrolled courses and progress
- Django admin panel
- SQLite database for easy local setup

## Setup (Windows / VS Code)
1. Install Python 3.10+.
2. Extract this ZIP and open the `lms_project` folder in VS Code.
3. Open Terminal and create a virtual environment:
   ```bash
   python -m venv venv
   ```
4. Activate it:
   ```bash
   venv\\Scripts\\activate
   ```
5. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
6. Create database tables:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```
7. Create an admin account:
   ```bash
   python manage.py createsuperuser
   ```
8. Start the server:
   ```bash
   python manage.py runserver
   ```
9. Open http://127.0.0.1:8000/

Admin panel: http://127.0.0.1:8000/admin/

## Instructor workflow
Register an account and choose **Instructor**. Use the instructor dashboard to create courses and add lessons.

## Notes
- This is a portfolio-ready MVP, not a production deployment. Before production, configure `DEBUG=False`, a secure `SECRET_KEY`, HTTPS, email verification, file storage, backups, and stronger authorization tests.
- SQLite is used by default. You can switch to PostgreSQL for deployment.
