# Ex02 Django ORM Web Application
# Date:30-09-2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM:
![alt text](<Screenshot 2024-12-06 224803.png>)
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM:
```
admin.py
from django.contrib import admin
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

models.py
from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
  name=models.CharField(max_length=100)
  accno=models.IntegerField(primary_key="accno")
  ifscno=models.IntegerField()
  mobno=models.IntegerField()
  email=models.EmailField()
   
class BankloanAdmin(admin.ModelAdmin):
  list_display=('name','accno','ifscno','mobno','email')
 
```
# OUTPUT
![django 2](https://github.com/user-attachments/assets/eb590d79-b816-42ee-bb1a-95f8af62854d)
![django 1](https://github.com/user-attachments/assets/312f151b-1988-4b02-a411-a6a3123d189f)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
