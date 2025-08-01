# LocalH System

LocalH System is a Django-based web application designed for managing doctor appointments, user registrations, and administrative tasks in a healthcare environment. The system supports multiple user roles (Admin, Doctor, Patient) and provides a modern, responsive interface for all users.

## Features

- **User Authentication**: Secure login and registration for doctors and patients.
- **Doctor Management**: Admins can add, update, and delete doctor profiles and specializations.
- **Appointment Booking**: Patients can book appointments with doctors, view their status, and receive prescriptions.
- **Doctor Dashboard**: Doctors can view, approve, cancel, and complete appointments, as well as add remarks and prescriptions.
- **Admin Dashboard**: Admins can manage doctors, specializations, and view reports.
- **Search & Reports**: Search appointments and generate reports between dates.
- **Responsive UI**: Built with Bootstrap and custom CSS for a modern look.

## Project Structure

- `dasapp/` - Main Django app with models and business logic
- `docappsystem/` - Project settings, views, and URL routing
- `media/` - Uploaded profile pictures and media files
- `static/` - Static assets (CSS, JS, images)
- `templates/` - HTML templates for all user roles

## Requirements

- Python 3.8+
- Django 3.2
- MySQL (or SQLite for development)
- See `requirements.txt` for all dependencies

## Setup Instructions

1. **Clone the repository**

2. **Install dependencies**

   ```powershell
   pip install -r requirements.txt
   ```

3. **Configure the database**

   - Update `docappsystem/settings.py` with your MySQL credentials.
   - Default DB: `docaspythondb` (see `DATABASES` section in settings).

4. **Apply migrations**

   ```powershell
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create a superuser (admin)**

   ```powershell
   python manage.py createsuperuser
   ```

6. **Run the development server**

   ```powershell
   python manage.py runserver
   ```

7. **Access the app**
   - Open your browser and go to `http://127.0.0.1:8000/`

## Usage

- **Admin Panel**: `/admin/` or via dashboard after login
- **Doctor Registration**: `/docsignup/`
- **Patient Appointment**: `/appointment/`

## License

This project is for educational purposes.
