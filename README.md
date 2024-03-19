# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-19 at 09 31 25_6bf68f39](https://github.com/thamizh610/ORM/assets/150418511/470173f4-e142-4b52-8602-26724b82d4fa)


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
from .models import railway,railwayAdmin
admin.site.register(railway,railwayAdmin)
models.py
from django.db import models
from django.contrib import admin
class railway (models.Model):
    train_code=models.CharField(max_length=20,help_text="railway train_code")
    train_name=models.CharField(max_length=100)
    start_time=models.IntegerField()
    End_time=models.IntegerField()
    start_station_code=models.IntegerField()
    end_station_code=models.IntegerField()
     
class railwayAdmin(admin.ModelAdmin):
    list_display=('train_code','train_name','start_time','End_time','start_station_code','end_station_code',)
```

## OUTPUT

![WhatsApp Image 2024-03-19 at 09 19 23_f2ef1ce2](https://github.com/thamizh610/ORM/assets/150418511/8343da48-d235-4b59-987c-4201f95b3e85)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
