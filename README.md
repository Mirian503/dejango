La aplicación no funcionará sin una base de datos, por lo que debes crear local_settings.py en la misma carpeta que settings.py. Yo uso Postgre, por lo que esta configuración es solo para Postgre.
El local_settings.py debe ser así:

DATABASES = {
    'default': {
        'ENGINE': "django.db.backends.postgresql",
        'NAME': 'db name',
        'USER': 'db_user',
        'PASSWORD': 'user password',
        'HOST': '127.0.0.1 (local host)',
        'PORT': '5432',
    }
}  
