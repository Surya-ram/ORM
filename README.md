# Django ORM Web Application
## Date:14-09-2023

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![ex 2](https://user-images.githubusercontent.com/128462891/236660168-dd95809a-c138-4f22-a1aa-bad7cac6b562.png)


Include your ER diagram here

## DESIGN STEPS

### STEP 1:
clone problem from github.
### STEP 2:
Create a new app.
### STEP 3:
Enter the code for admin.py and models.py.
### step 4:
Create django app and add student details.

## PROGRAM
```python
from django.db import models
from django.contrib import admin
class GitDatabase(models.Model):
    username_primary_key = models.CharField(max_length=30, help_text="User name must be unique", primary_key=True,unique=True)
    password = models.CharField(max_length=30)
    firstname = models.CharField(max_length=20)
    lastname = models.CharField(max_length=20)
    profile_photo = models.ImageField()
    email = models.EmailField(max_length=50,unique=True)
class GitAdmin(admin.ModelAdmin):
    list_display = ('username_primary_key', 'password', 'firstname', 'lastname','profile_photo','email')
 ```

Include your code here

## OUTPUT

![Screenshot 2023-05-07 111902](![240855977-229d0234-cc21-42a1-afb5-892c6a82df8b](https://github.com/Surya-ram/ORM/assets/122000311/9a2b2728-c779-4dbf-b562-853299069606)
)


## RESULT
Thus a Django application is successfully developed to store and retrive data from a database using object realtion mapping
