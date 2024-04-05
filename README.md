# Ex02 Django ORM Web Application
## Date: 
 05/04/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

This is my ER Diagram


![WEB](https://github.com/vaishnavidevi23013992/ORM/assets/151864235/28e98abf-2f0c-4c2a-b433-190c6e6592fe)


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

DEVELOPER NAME : VAISHNAVIDEVI V

REGISTER NUMBER: 212223040230


## models.py:
```
from django.db import models
from django.contrib import admin
class Book(models.Model):
    book_id=models.IntegerField()
    book_name=models.CharField(max_length=100)
    page=models.IntegerField()
    price=models.IntegerField()
    author=models.CharField(max_length=30)


class BookAdmin(admin.ModelAdmin):
    list_display=('book_id','book_name','page','price','author')
```
## admin.py:
```
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```
## OUTPUT
![webb](https://github.com/vaishnavidevi23013992/ORM/assets/151864235/ce7ec008-de1f-44db-8594-39060bfd7381)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
