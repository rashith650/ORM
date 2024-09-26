# Ex02 Django ORM Web Application
## Date:26/09/24 

## AIM
To develop a Django application to store and retrieve data from a Train database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="493" alt="315949707-cf94daf7-9d13-4ec6-8691-3c3db8533e7e" src="https://github.com/user-attachments/assets/37d1b237-273b-446a-9bba-df08fef4d5e6">

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
```
from django.contrib import admin

from .models import Train, TrainAdmin

admin.site.register(Train, TrainAdmin)
```

models.py
```
from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.DateTimeField()
    End_time=models.DateTimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')
```
## OUTPUT
![Screenshot 2024-09-26 061018](https://github.com/user-attachments/assets/a6e6cde7-3b55-4558-a2fb-a4c18baa9b31)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
