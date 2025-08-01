🏥 LocalH System – Telemedicine Reimagined for Local Communities
LocalH is a Django-based telemedicine web application tailored for localized healthcare management. It empowers patients, doctors, and admins with a seamless system to manage appointments, prescriptions, and reporting—all under one roof.

Built to support county health systems and rural hospitals, LocalH bridges the gap between remote communities and specialist care.

✨ Features
✅ Multi-role Access System

Admins, Doctors, and Patients each have their own dashboards and permissions.

✅ Smart Appointment Management

Patients choose doctors by specialty and book time slots.

Doctors can accept, decline, complete, or prescribe post-visit.

Admins view all appointments and filter by date.

✅ Specialist Search

Patients can filter doctors by specialty, making the platform ideal for referrals and teleconsults.

✅ Prescriptions & Medical Notes

Doctors add visit remarks and downloadable prescriptions.

Patients receive prescriptions in their portal.

✅ Admin Reporting

Generate appointment reports between date ranges.

Track doctor performance and appointment trends.

✅ Modern Responsive UI

Built with Bootstrap for full mobile responsiveness.

Clean and intuitive design for accessibility across age groups.

✅ Secure User Authentication

Django's built-in auth system with hashed passwords and session protection.

🛠 Tech Stack
Tool	Purpose
Python 3.8+	Core programming language
Django 3.2	Web framework (backend + auth)
MySQL/SQLite	Database
Bootstrap	Frontend styling
HTML/CSS	UI templating and styling

📁 Project Structure
php
Copy
Edit
├── dasapp/              # Main Django app (models, views, templates)
├── docappsystem/        # Django project settings and URLs
├── media/               # Uploaded doctor/patient profile images
├── static/              # CSS, JS, and frontend assets
├── templates/           # HTML templates for all user roles
├── requirements.txt     # Python dependencies
🚀 Installation & Setup
Clone the repo

bash
Copy
Edit
git clone https://github.com/pinchase/localh-system.git
cd localh-system
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Configure DB

In docappsystem/settings.py, update:

python
Copy
Edit
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'docaspythondb',
        'USER': 'your-username',
        'PASSWORD': 'your-password',
        ...
    }
}
Migrate and start server

bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
Create a superuser

bash
Copy
Edit
python manage.py createsuperuser
Visit in browser

cpp
Copy
Edit
http://127.0.0.1:8000/
🎯 Access Points
Role	URL
Admin	/admin/ or /dashboard/
Doctors	/docsignup/
Patients	/appointment/

📈 Future Features (Planned for County Integration)
📞 Video Consultation (Twilio/Zoom API)

💊 E-Prescription Fulfillment Integration

🧠 Mental Health Chatbot Module

📱 Mobile App (Flutter/PWA)

🧾 SMS Notifications (Twilio, Africa’s Talking)

📍 Clinic Geo-mapping with GPS directions

📜 License
This project is currently open for educational and pilot deployment purposes.
All rights reserved © 2025.

🙌 Author & Maintainer
👨‍💻 Pinchase Kagiri
ICT Student | Software Engineer in Progress | Murang’a Native
🚀 Building tech that works for everyday Kenyans.
