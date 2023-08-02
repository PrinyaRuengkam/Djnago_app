# Django

## การสร้าง Project
    django-admin startproject *ขื่อโปรเจ็ค*

## การสร้าง Virtual Environment
    python -m venv env

## การรัน Server Django
    python manage.py runserver

## การสร้าง Admin register 
```python
from django.contrib import admin

# Register your models here.
from . import models


@admin.register(models.Student)
class StudentAdmin(admin.ModelAdmin):
    list_display = (
        'prefix',
        'std_id',
        'first_name',
        'last_name',
        'phone',
     
    )


```