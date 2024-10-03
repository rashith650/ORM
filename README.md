# Ex02 Django ORM Web Application
## Date: 03-10-2024
## NAME: MOHAMED RASHITH S
## REGISTER NO: 24001082

## AIM
To develop a Django application to store and retrieve data from a Bank database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![BA](https://github.com/user-attachments/assets/fc027c76-1cd5-4322-84ae-314ad52a3fb3)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 customers.

## PROGRAM

admin.py:
```
from django.contrib import admin
from .models import Bankloan, BankloanAdmin  
admin.site.register(Bankloan, BankloanAdmin)
```
models.py:
```
from django.db import models
from django.contrib import admin
from django.db import models
from django.contrib import admin

class Bankloan(models.Model):
    customerid= models.IntegerField(primary_key=True)
    customerrate = models.IntegerField()
    age = models.IntegerField()  
    cust_no = models.IntegerField()
    customerloan_purpose =models.CharField(max_length=500)

class BankloanAdmin(admin.ModelAdmin):
    list_display = ('customerid', 'customerrate', 'age', 'cust_no', 'customerloan_purpose')
```

## OUTPUT


![BANK IMG](https://github.com/user-attachments/assets/ecf232e6-84ac-40d1-9b7e-ade1cdde3bfb)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully

