# Ex02 Django ORM Web Application
## Date:26/09/24 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-09-26 161605](https://github.com/user-attachments/assets/7a6f9641-1321-4d80-982c-2bba81207616)


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

```
admin.py

from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno")
      name=models.CharField(max_length=50)
      author=models.CharField(max_length=70)
      price=models.IntegerField()
      publisher=models.CharField(max_length=60)

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher")

```
## OUTPUT
![Screenshot 2024-09-26 161642](https://github.com/user-attachments/assets/1513a17a-7f68-4111-9174-6ea0d9016bfa)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
