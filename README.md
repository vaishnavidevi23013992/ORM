# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

DEVELOPED BY:VAISHNAVIDEVI V
REG NO:212223040230
```
models.py
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    eid=models.CharField(max_length=20,help_text='Employee_ID')
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```

## OUTPUT
![EXP-2](https://github.com/vaishnavidevi23013992/ORM/assets/151864235/094350fa-c8d5-4277-b488-5c8f03c4bc57)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
