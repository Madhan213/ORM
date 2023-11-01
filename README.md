# Ex02 Django ORM Web Application
## Date: 28/10/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

```
Admin.py

from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)

Models.py  

from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Goals=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Goals','Position')


```

## OUTPUT

![Screenshot 2023-11-01 091420](https://github.com/Madhan213/ORM/assets/130206230/b0391ffc-2176-4c93-8aa7-44064037335f)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
