# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py code;
```
from django.db import models
from django.contrib import admin
class Car(models.Model):
    car_id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=50)
    model = models.CharField(max_length=50)
    year = models.DateField()
    price = models.IntegerField()

class CarAdmin(admin.ModelAdmin):
    list_display=('car_id','brand','model','year','price')
```
admin.py code;
```
from django.contrib import admin
from .models import Car,CarAdmin

admin.site.register(Car,CarAdmin)
```

## OUTPUT
<img width="1918" height="1087" alt="exp2 ss" src="https://github.com/user-attachments/assets/d2b591f5-185b-457a-a5bc-10308bc5e345" />


Include the screenshot of your admin page.


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
