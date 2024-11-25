# Ex02: Django ORM Web Application
## Date: 24-11-2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/1e4280ad-db40-46b7-b582-bb3f121e4c11)


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

admin.py

from django.contrib import admin

from .models import Bankloan,BankloanAdmin

admin.site.register(Bankloan,BankloanAdmin)

model.py
from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
    date_of_birth=models.DateField(default=0)
    fathers_name=models.CharField(max_length=70,default=0)
    age=models.IntegerField(default=0)
    customerid=models.IntegerField(primary_key="customerid",default=0)
    accountdetails=models.CharField(max_length=70,default=0)

    class BankloanAdmin(admin.ModelAdmin):
    list_display=('date_of_birth','fathers_name','age','customerid','accountdetails')




## OUTPUT

Include the screenshot of your admin page.

![Screenshot 2024-11-24 191705](https://github.com/user-attachments/assets/dc487b3a-473b-480d-a946-daf53425e213)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
