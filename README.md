# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ent](https://github.com/Tanug25/django-orm-app/assets/138849166/502786fc-e79c-4802-9f46-a7b31b6ca7bf)


## DESIGN STEPS

### STEP 1:
creating a table using required details in Django-ORM
### STEP 2:
upload the python code.
### STEP 3:
push the code to github

## PROGRAM
```html
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(primary_key=True,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    number=models.IntegerField()
class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email','number')
    ```

### admin.py
```html
from django.contrib import admin
from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)
```
## OUTPUT

![out1](https://github.com/Tanug25/django-orm-app/assets/138849166/3a69da87-4412-45c8-8453-d7a7038283dd)

![out2](https://github.com/Tanug25/django-orm-app/assets/138849166/1433408b-a39b-485c-819d-578207fc2bb4)

## RESULT
The above program is executed successfully.
