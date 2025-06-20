# Ex02 Django ORM Web Application
## Date: 19/03/2024

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).


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
models.py
from django.db import models

from django.contrib import admin



class Employee(models.Model):

    emp_id = models.IntegerField(primary_key=True)

    emp_name = models.CharField(max_length=50)

    phone = models.BigIntegerField()

    email = models.EmailField()

    department = models.CharField(max_length=30)

    salary = models.DecimalField(max_digits=10, decimal_places=2)

    joining_date = models.DateField()



class EmployeeAdmin(admin.ModelAdmin):

    list_display = ('emp_name', 'department', 'email', 'salary')

```

## OUTPUT
![alt text](<Screenshot (117).png>)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
