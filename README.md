# Ex02 Django ORM Web Application
# Date:27:9:2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![{F1018B2F-8DAB-4608-9C8B-CCABCA8B89A0}](https://github.com/user-attachments/assets/964a46f9-d25b-4802-a623-6ac4519ffb4d)


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

1.models.py
```
from django.db import models
from django.contrib import admin

class Book(models.Model):
    book_no = models.CharField(max_length=100, primary_key=True)
    book_name = models.CharField(max_length=100)
    name = models.CharField(max_length=100)
    mobile_no = models.CharField(max_length=15)
    email = models.EmailField()
    aadhar_no = models.CharField(max_length=12)
    address = models.CharField(max_length=255)
    Institute_name=models.CharField(max_length=100)

class BookAdmin(admin.ModelAdmin):
    list_display = ('book_no', 'book_name', 'name', 'mobile_no', 'email','aadhar_no','address','Institute_name')

```
2.admin.py
```
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)

```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot (197)](https://github.com/user-attachments/assets/8a2dbe8c-679d-466c-a9a8-bc5d0608c56c)


![Screenshot (198)](https://github.com/user-attachments/assets/c2d806d3-11dd-4607-a6c9-f82020e8c572)
![{4A47FDCF-0BB0-44F5-A4C7-D82879DE80A7}](https://github.com/user-attachments/assets/e91b6e18-64ca-4747-8559-c46a8c630407)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
