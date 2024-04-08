# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Student database using Object Relational Mapping(ORM).

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

# models.py
```
from django.db import models
from django.contrib import admin
class Student(models.Model):
    studid=models.IntegerField()
    studname=models.CharField(max_length=20)
    dept=models.CharField(max_length=20)
class StudentAdmin(admin.ModelAdmin):
    list_display=('studid','studname','dept')
```
# admin.py
```
from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```
## OUTPUT

![ORM](https://github.com/Isreal129/ORM/assets/125784931/6b6cae41-273e-45cc-846f-1cf6f7d18d56)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
