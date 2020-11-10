# docker-compose-networking
Learn-docker-compose-networking. Django sample here: https://docs.docker.com/compose/django/

# $ git remote add github-docker-compose-networking https://github.com/gopinaath/docker-compose-networking.git

# $ git push github-docker-compose-networking master


# $ sudo docker-compose run web django-admin startproject composeexample .
# sudo chown -R $USER:$USER .

In your project directory, edit the composeexample/settings.py file.

Replace the DATABASES = ... with the following:

\# settings.py
```json   
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',
        'USER': 'postgres',
        'PASSWORD': 'postgres',
        'HOST': 'db',
        'PORT': 5432,
    }
}
```

ALLOWED_HOSTS = ['*']

# $ docker-compose up

# http://localhost:8000

# $ docker-compose down
