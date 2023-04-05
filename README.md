# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github
### STEP 2:
creat a new app
### STEP 3:
Enter the code for admin.py and model.py
## PROGRAM
```python
from django.db import models

from django.contrib import admin

class Student (models.Model):
     referencenumber=models.CharField(max_length=20,help_text="reference number")
     name=models.CharField(max_length=100)
     age=models.IntegerField()
     email=models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```

## OUTPUT
![Screenshot 2023-04-01 083939](https://user-images.githubusercontent.com/117974950/229989545-d0fb05e7-67df-4092-8db6-d75bdb735eee.png)
![Screenshot 2023-04-01 085806](https://user-images.githubusercontent.com/117974950/229989567-443ac71b-36c6-4168-8e28-9e4d968014ab.png)

## RESULT
The program is executed succesfully
