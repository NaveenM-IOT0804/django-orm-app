# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1: Clone the problem from github
### STEP 2: creat a new app
### STEP 3: Enter the code for admin.py and model.py
## PROGRAM
```python
from django.db import models
from django.contrib import admin
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    gender=models.CharField(max_length=100)

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','gender')
```

## OUTPUT
### Server Output:
![image](https://user-images.githubusercontent.com/117974950/230269934-26b5ace9-a9b4-4ffb-b30f-3445dad8b405.png)
### Client Output:
![Screenshot 2023-04-06 092332](https://user-images.githubusercontent.com/117974950/230270012-169f0d52-9b67-45e8-be0b-c0e8e8d475b9.png)
![Screenshot 2023-04-06 093408](https://user-images.githubusercontent.com/117974950/230270037-ea125b5b-4d60-47a2-8b89-25512afeb351.png)


## RESULT
The program is executed succesfully
