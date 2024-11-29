# Ex02 Django ORM Web Application
# Date:29:11:2024
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
```
1.models.py

from django.db import models
from django.contrib import admin

class Book(models.Model):
    book_no = models.CharField(max_length=100)
    book_name = models.CharField(max_length=100)
    name = models.CharField(max_length=100)
    mobile_no = models.CharField(max_length=15)
    email = models.EmailField()
    aadhar_no = models.CharField(max_length=12)
    address = models.CharField(max_length=255)

class BookAdmin(admin.ModelAdmin):
    list_display = ('book_no', 'book_name', 'name', 'mobile_no', 'email','aadhar_no','address')

2.admin.py

from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)

```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot (163)](https://github.com/user-attachments/assets/3b5d7f08-4780-4707-b2e6-db45647e4eda)

![Screenshot (164)](https://github.com/user-attachments/assets/9aca72ba-771d-47a5-96c8-4d341c6373cf)



![{6B5672F7-4C1E-4796-BF4D-467ECA1A1902}](https://github.com/user-attachments/assets/f9844b1f-613c-4577-91b8-45d734604437)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
