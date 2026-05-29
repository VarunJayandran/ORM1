# Ex01 Django ORM Web Application
# Date:29-05-2026
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
models.py
from django.db import models
from django.contrib import admin
class product(models.Model):
    productname=models.CharField(max_length=30)
    category=models.CharField(max_length=15)
    productbrand=models.CharField(max_length=20)
    Dateofpack=models.DateField()
    Dateofdeli=models.DateField()
    price=models.IntegerField()
    productID=models.CharField(primary_key=True,max_length=15)

class productadmin(admin.ModelAdmin):
    list_display=["productID","productname","category","productbrand","Dateofpack","Dateofdeli","price"]

admin.py

from django.contrib import admin
from .models import product,productadmin
admin.site.register(product,productadmin)
```
# OUTPUT

![alt text](<Screenshot 2026-05-29 094804.png>)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
![alt text](<Screenshot 2026-05-29 094804.png>)