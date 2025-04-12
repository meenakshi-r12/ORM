# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM


![Screenshot (5)](https://github.com/user-attachments/assets/86f5e4fd-7b7d-4639-8ab1-e0f865cadef3)

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
class BankLoan(models.Model):
    Name = models.CharField(max_length=100)
    Account_No = models.IntegerField(primary_key="Account_No")
    Phone_Number = models.IntegerField()
    Aadhar_No = models.IntegerField()
    Loan_amount = models.FloatField()
    Time_Period = models.IntegerField()
     
class BankAdmin(admin.ModelAdmin):
    list_display = ('Name', 'Account_No', 'Phone_Number','Aadhar_No', 'Loan_amount', 'Time_Period',)


admin.py


from django.contrib import admin
from .models import BankLoan,BankAdmin 
admin.site.register(BankLoan,BankAdmin)

```

## OUTPUT

Include the screenshot of your admin page.

![Screenshot (4)](https://github.com/user-attachments/assets/fd9c38ee-652d-4473-b958-70bdfe5e2c42)

## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
