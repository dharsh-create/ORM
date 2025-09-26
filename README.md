# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![WhatsApp Image 2025-09-26 at 8 29 43 AM](https://github.com/user-attachments/assets/eb831aa2-aa51-433c-ba23-dc7d06c402a6)


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
from .models import Movies, MoviesAdmin
admin.site.register(Movies,MoviesAdmin)


models.py

from django.db import models
from django.contrib import admin
class Movies(models.Model):
    M_ID = models.IntegerField(primary_key=True)
    M_name = models.CharField(max_length=100)
    Release_date=models.DateField()
    Director=models. CharField(max_length=50)
    Actors=models. CharField(max_length=100)
 
class MoviesAdmin(admin.ModelAdmin):
    list_display=('M_ID','M_name','Release_date', 'Director','Actors')
```

## OUTPUT


![WhatsApp Image 2025-09-26 at 8 12 11 AM](https://github.com/user-attachments/assets/affc2850-2a8c-4a22-8de5-15b104d0149c)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
