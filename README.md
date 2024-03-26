# Learning-Django
Path to become a django expert

In this path, we are going to build College Management System using Django and will be using dbsqlite database. In the times of covid, when education has totally become digital, there comes a need for a system that can connect teachers, students, and HOD and that was the motivation behind building this project.
This project allows HOD, staff, and students to register themselves. This project has three interfaces.

Tools and Technologies Used in the Project:
HTML
CSS
JAVASCRIPT
JQUERY
BOOTSTRAP
DJANGO

Required Skillset to Build the Project:
Basic knowledge of HTML, CSS, JavaScript, and Django.

Step By Step Implementation
Follow the below steps to implement the project:

Step 1: Install and deploy the Django project's environnement

Create a folder with the name of the Django Project (College_Management_System).
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/aafa487f-181d-48c1-90d7-a3be059815ed)

Open your favorite IDE (mine is PyCharm) and select File > Open... from the menu,
Navigate to the College_Management_System folder you created and open it.
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/470bc0cc-30e7-4437-9889-9053caa410a1)

Set Up a Virtual Environment:
In PyCharm, i open the Terminal (usually at the bottom of the IDE).
Run the following command to create a virtual environment:

python -m venv "nameofyourvenv"

Once the virtual environment is created, activate it:
As i use a Windows Computer, i will type:

nameofyourvenv\Scripts\activate

Install Django:
With the virtual environment activated, install Django using PyCharm’s Terminal:

pip install django
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/3dfb274f-cfef-449e-9491-525002ec24a2)

Create a New Django Project:
Still in the Terminal, run the following command to create a new Django project:

django-admin startproject nameofyourproject
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/3da08e95-8ef7-4605-9ae2-c80504f4f6b0)

This will create a new Django project with the name nameofyourproject inside your College_Management_System folder.
Open the Django Project:
In PyCharm, right-click on the nameofyourproject folder and select Mark Directory as > Sources Root. This helps PyCharm recognize it as the main project folder.
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/90879082-b3dd-4b7a-be11-592de3dedf2a)

Run the Development Server:
To make sure everything is set up correctly, you can run Django’s development server:

python manage.py runserver
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/940ea8c0-8df5-4ac5-a35c-7c9df9e83918)

Open your web browser and go to http://127.0.0.1:8000/ or http://localhost:8000/ to see the default Django welcome page.
![image](https://github.com/JPK2001/Learning-Django/assets/115308301/892c0ddf-2bff-453e-9477-c739185f5d8e)

Step 2: 
