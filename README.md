# Student Result Management System (Django)

**Author:** Taha Nawaz  
 

---

## Overview
This is a simple Django web application to manage **student records** using `ModelForm`.  
The project allows performing all **CRUD operations**: Create, Read, Update, Delete.

---

## Features
- Add new students  
- View all students  
- Update existing student details  
- Delete student records after confirmation  

---

## Technologies Used
- Python 3.x  
- Django 4.x  
- HTML (Django Templates)  
- SQLite (default Django database)  

---

## Project Structure
studentproject/
├── studentproject/
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
├── students/
│ ├── models.py # Student model
│ ├── forms.py # ModelForm for Student
│ ├── views.py # CRUD views
│ ├── urls.py # App URLs
│ └── templates/students/
│ ├── student_list.html
│ ├── student_form.html
│ └── student_confirm_delete.html
├── manage.py
└── README.md

---

## Setup Instructions

### 1. Create virtual environment
```bash
python -m venv myenv
# Activate environment:
# Linux / Mac
source myenv/bin/activate
# Windows
myenv\Scripts\activate
pip install django
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
