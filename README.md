# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

Create django application

### STEP 2:

Write code in models.py and admin.py

### STEP 3:

End of the program


## PROGRAM
## Models.py:
```python
from django.db import models
from django.contrib import admin

# Create your models here.

class Student (models.Model):
    referencenumber=models.CharField(max_length=20,primary_key=True,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    department=models.CharField(max_length=30)


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','department'

```
## Admin.py
```python
from django.contrib import admin
from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)
```
## OUTPUT
## server output:


## client output:



## RESULT
Thus the program has been executed successfully
