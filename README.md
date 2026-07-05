# College ERP System (SPPU University)

A comprehensive, role-based College Enterprise Resource Planning (ERP) System built with Python, Django, and MySQL. This system facilitates seamless collaboration and administrative management across HODs (Admins), Staff, and Students.

---

## 🚀 Features

### 👨‍💼 HOD (Admin) Panel
* **Staff & Student Management:** Add, update, and manage staff and student profiles.
* **Course & Subject Allocation:** Add courses, subjects, and assign them to respective staff members.
* **Attendance Monitoring:** View overall student attendance logs.
* **Leave Requests:** Approve or reject leave applications from staff and students.
* **Feedback Systems:** View feedback messages sent by staff/students and reply to them.
* **Notifications:** Send system notifications directly to staff and students.

### 👩‍🏫 Staff Panel
* **Attendance Management:** Take attendance for assigned subjects and update/modify records.
* **Academic Marks:** Add and edit academic results (Assignment and Exam marks) for students.
* **Leave Applications:** Apply for leave and track approval status.
* **Feedback:** Send feedback messages directly to the HOD.
* **Live Classroom:** Start live virtual class sessions.

### 🎓 Student Panel
* **Attendance Tracking:** View subject-wise attendance percentage and logs.
* **View Results:** Securely check assignment and exam results posted by staff.
* **Leave Applications:** Submit leave requests directly to the HOD.
* **Feedback System:** Submit queries or feedback to the college management.

---

## 🛠️ Tech Stack

* **Backend:** Python 3.11+, Django 5.2
* **Database:** MySQL
* **Frontend:** AdminLTE 3 (Dashboard Template), Bootstrap 4, HTML5, CSS3
* **Interactions:** jQuery, AJAX (CSRF Secured)

---

## ⚙️ Installation & Setup

Follow these steps to run the application locally:

### 1. Clone the Repository
```bash
git clone https://github.com/ShravanManekar/College_ERP_System.git
cd College_ERP_System
```

### 2. Install Dependencies
Make sure you have Python installed, then run:
```bash
pip install -r requirements.txt
```

### 3. Configure the Database
1. Open your MySQL client and create a database named `college_erp`:
   ```sql
   CREATE DATABASE college_erp CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
   ```
2. Update the `DATABASES` settings in `student_management_system/settings.py` with your MySQL root credentials if different:
   ```python
   DATABASES = {
       'default': {
           'ENGINE': 'django.db.backends.mysql',
           'NAME': 'college_erp',
           'USER': 'root',
           'PASSWORD': 'YOUR_PASSWORD',
           'HOST': 'localhost',
           'PORT': '3306',
       }
   }
   ```

### 4. Run Database Migrations
Apply the migrations to set up database tables:
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create a Superuser (Admin)
Create an admin account to access the HOD panel:
```bash
python manage.py createsuperuser
```

### 6. Run the Development Server
```bash
python manage.py runserver
```
Visit the application in your browser: **http://127.0.0.1:8000/**

---

## 👥 Contributors

* **Shravan Manekar** — Lead Developer & Repository Owner
