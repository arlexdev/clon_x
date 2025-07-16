# clon_x
para la instalacion del proyecto se necesitara las siguientes herramientas
1. instalacion de python
2. instalacion de node.js
creacion de entorno virtual para el proyecto
    python -m venv venv
instalacion de django
    pip install django
instalacion de paquete django-tailwind
    python -m pip install django-tailwind
En el archivo settings.py agregar aplicacion
    INSTALLED_APPS = [
    # other Django apps
    'tailwind',
    ]
iniciar tailwind
    python manage.py tailwind init

en aplicaciones agregar 'theme'
    INSTALLED_APPS = [
    # other Django apps
    'tailwind',
    'theme'
    ]
en el mismo archibo settings.py agregar
    TAILWIND_APP_NAME = 'theme'
    INTERNAL_IPS = ["127.0.0.1"]
    NPM_BIN_PATH = 'C:/Program Files/nodejs/npm.cmd'
luego en terminal
    python manage.py tailwind install\
