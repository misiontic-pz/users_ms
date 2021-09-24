###Activate Env
source env/bin/activate
___

###Run server
python manage.py runserver
___

DB connection
usersProject/settings.py -> DATABASES


###Files to modify
- serializers.py  (New file)
- views.py
- urls.py

###Migrations
- python manage.py makemigrations
- python manage.py migrate

###Reset Migrations (DB)
- Delete 'migrations' folder
- python manage.py migrate admin zero
- python manage.py migrate auth zero
- python manage.py migrate contenttypes zero
- python manage.py migrate sessions zero

###Superusers
- python manage.py createsuperuser

###Deplyment Heroku
- heroku login
- heroku container:login
- heroku container:push web --app misiontic-ms-users
- heroku container:release web --app misiontic-ms-users