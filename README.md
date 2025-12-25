# College-ERP
A college management system built using Django framework. It is designed for interactions between students and teachers. Features include attendance, marks and time table.

## Installation

Python and Django need to be installed

```bash
pip install python
pip install django
pip install -r requirements.txt

```
## Virtual Environment Setup
To start project first start virtual environment and terminal should look like this:

(venv) PS C:\Users\College-ERP\College-ERP-master>

For this you have to follow :
Go to folder
Open College-ERP
Open College-ERP-master
And run on terminal
```
venv\scripts\activate
py manage.py makemigrations
py manage.py migrate
```
```bash 
Then runserver :
python manage.py runserver
```

Then go to the browser and enter the url **http://127.0.0.1:8000/**


## Login

The login page is common for students and teachers.  
The username is their name and password for everyone is 'project123'.  

Example usernames:  
student- 'Durgesh'  


You can access the django admin page at **http://127.0.0.1:8000/admin** and login with username 'admin' and the above password.

Also a new admin user can be created using

```bash
python manage.py createsuperuser
```

## Users

New students and teachers can be added through the admin page. A new user needs to be created for each. 

The admin page is used to modify all tables such as Students, Teachers, Departments, Courses, Classes etc.



## Update (29/01/2024)

Added method to reset attendance time range in Django Admin page.

![alt_text](https://i.imgur.com/0xOWmUZ.png)

This is present in Django Admin -> Attendance (http://127.0.0.1:8000/admin/info/attendanceclass/).  
Start Date: Start Date of Attendance period  
End Date: End Date of Attendance period

This will delete all present attendance data and create new attendance objects for the given time range. 
