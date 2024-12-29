# Ex02 Django ORM Web Application
# Date:15/11/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
admin.py
```
from django.contrib import admin
from .models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)
```
models.py
```
from django.db import models
from django.contrib import admin
class Loan(models.Model):
    Customerid=models.CharField(max_length=20, primary_key=True)
    Customername=models.CharField(max_length=100)
    Mobile=models.IntegerField( )
    Age=models.IntegerField( )
    Email=models.EmailField( )
    DOB=models.DateField( )
    Loan_amount=models.IntegerField( )
class LoanAdmin(admin.ModelAdmin):
    list_display=('Customerid','Customername','Mobile','Age','Email','DOB','Loan_amount')
```
# OUTPUT
![loan](https://github.com/user-attachments/assets/314487a8-ef80-4393-8c30-e2b435933ebc)
![loan 2](https://github.com/user-attachments/assets/eb52a7d6-52e9-4999-ae84-099fe43d7253)
![loan 3](https://github.com/user-attachments/assets/0ecfe9f2-62b7-456a-b6e4-387224f42fbc)
![Screenshot 2024-12-12 132812](https://github.com/user-attachments/assets/661db09a-24f1-4d17-8174-16906a82640b)
# ER DIAGRAM
![Untitled](https://github.com/user-attachments/assets/27d3f6fe-25e9-4beb-bbe2-2447e94f6f6a)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
