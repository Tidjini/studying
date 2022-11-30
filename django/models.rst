MODELS NOTES
*****************

- django use an API for databases to filter, and perform CRUD operation, even though you can use sql queries to manage database.
- models should be clean from import, especially with importing views or other top level imports.
- Modelisation is very important in this stage **[STRUCTURAL PATTERN]** with 1st, 2dn, 3rd normal forms.
- Model **Mixin**, to apply **DRY PRINCIPAL** :
    - Django **abstract model**, using the Meta subclass to define it:
        
        .. code-block:: python
            :linenos:
            :emphasize-lines: 4-5
            form django.db import models

            class TimespanModel(models.Model):
                created_at = model.DateTimeField(auto_add_now=True)
            
                class Meta:
                    # this should tell django to not create this Model as concreat table (not a persistant) 
                    abstract = True
                
        
    - abstract models:
        - can not be instantiate
        - have no Foreign Key or Many to Many Relation
        - can not be query directly

- You can seperate your models into differents files, you should create **models package** with **__init__.py** file inside your application.

- For Postger ArrayField, must Install **psycopg2**
- For ImageField, must install **pillow**