# Django Helpful Snippets


## Getting your environment setup

    $ pipenv install # Will create virtual env first time
    $ pipenv shell # Log into the virtual environment
    $ python manage.py migrate # Only have to run this when there are migrations to run
    $ python manage.py runserver

## Deleting records for a single model

    $ python manage.py shell
    $ from {{app name}}.models import {{model name}}
    
    $ data_to_be_deleted = {{model name}}.objects.all()
    $ data_to_be_deleted.delete()
    
    ### you can also run it in a single line ###
    $ {{model name}}.objects.all().delete()
