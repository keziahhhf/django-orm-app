# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py



## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Football,FootballAdmin
admin.site.register(Football,FootballAdmin)

models.py

from django.db import models
from django.contrib import admin
class Football (models.Model):
    player_name=models.CharField(max_length=20)
    age=models.IntegerField()
    score=models.IntegerField()
    email=models.EmailField()
    date=models.DateField()
    
class FootballAdmin(admin.ModelAdmin):
    list_display=('player_name','age','score','email','date')
```


## OUTPUT

![screenshot jpg](https://github.com/keziahhhf/django-orm-app/assets/155235704/3e9c2a9b-4f3f-4ce2-a4bc-5b212fb14cd2)




## RESULT
