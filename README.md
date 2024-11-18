# Ex02 Django ORM Web Application
## Date:17-11-24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![alt text](<Screenshot 2024-11-18 113659.png>)


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
'''
admin.py

from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)

models.py

from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    loan_id = models.IntegerField(primary_key=True)
    loan_type = models.CharField(max_length=60)
    loan_amt = models.IntegerField()
    cust_name = models.CharField(max_length=30)
    cust_acno = models.IntegerField()
class bankloanAdmin(admin.ModelAdmin):
    list_display = ('loan_id','loan_type','loan_amt','cust_name','cust_acno')
                         


'''


## OUTPUT

![alt text](<Screenshot (7).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
