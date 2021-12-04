## Django introduction:
![](https://files.realpython.com/media/Get-Started-With-Django_Watermarked.15a1e05597bc.jpg)


### What is Django?
- Django is a high-level Python web framework that enables rapid development of secure and maintainable websites.
- It is free and open source, has a thriving and active community, great documentation, and many options for free and paid-for support
- Django was initially developed between 2003 and 2005 by a web team who were responsible for creating and maintaining newspaper websites


##### Models:
- A model is the single, definitive source of information about your data.
-  It contains the essential fields and behaviors of the data you’re storing. Generally, each model maps to a single database table
- Each model is a Python class that subclasses django.db.models.Model.
- Each attribute of the model represents a database field.
- With all of this, Django gives you an automatically-generated database-access API; see Making queries.

- This example model defines a Person, which has a first_name and last_name:
 ```
 from django.db import models

class Person(models.Model):
    first_name = models.CharField(max_length=30)
    last_name = models.CharField(max_length=30)
```

##### URLs and views:
- A clean, elegant URL scheme is an important detail in a high-quality web application.
- Django encourages beautiful URL design and doesn’t put any cruft in URLs, like .php or .asp.
 ```
 from django.urls import path

from . import views

urlpatterns = [
    path('bands/', views.band_listing, name='band-list'),
    path('bands/<int:band_id>/', views.band_detail, name='band-detail'),
    path('bands/search/', views.band_search, name='band-search'),
]
```
##### Templates:
- Django’s template language is designed to strike a balance between power and ease. It’s designed to feel comfortable and easy-to-learn to those used to working with HTML, like designers and front-end developers.
-  But it is also flexible and highly extensible, allowing developers to augment the template language as needed.
##### Forms
- Django provides a powerful form library that handles rendering forms as HTML, validating user-submitted data, and converting that data to native Python types.
- Django also provides a way to generate forms from your existing models and use those forms to create and update data.

###### Django’s code is open source and available to all. Django’s organization is managed by a non-profit, the DSF, with a miniscule budget. And Django code is lead by a core team of volunteers, two paid Django Fellows, and a larger group of contributors.
