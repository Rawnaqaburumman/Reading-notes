# Model:
 Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc.
 
 ### Designing the LocalLibrary models:
 - We know that we need to store information about books (title, summary, author, written language, category, ISBN)
 - When designing your models it makes sense to have separate models for every "object"
 - we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).

# Model definition:
- Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata

# Creating a superuser:
![](https://simpleisbetterthancomplex.com/media/series/beginners-guide/1.11/part-2/Pixton_Comic_Django_Admin.png)

- You can create a "superuser" account that has full access to the site and all needed permissions using manage.py.

## Logging in and using the site:
- To login to the site, open the /admin URL (e.g. http://127.0.0.1:8000/admin) and enter your new superuser userid and password credentials (you'll be redirected to the login page, and then back to the /admin URL after you've entered your details).
-  You can click on a model name to go to a screen that lists all its associated records, and you can further click on those records to edit them. You can also directly click the Add link next to each model to start creating a record of that type.
