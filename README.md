# Backend API Project - Django REST Framework

## Descripcion
Proyecto de la materia backend 3 usando DJango y Django Rest Framework haciendo uso de buenas practicas.

## Tecnologias
- Python
- Django
- Django REST framework

## Clonar repositorio
```bash
# HTTPS
git clone https://github.com/Derian-18/REST.git
```

```bash
# SSH
git clone git@github.com:Derian-18/REST.git
```

## Intalar dependencias
```bash
pip install -r requirements.txt
```

## Cambiar development por prodution

```bash
# cambiar a produccion
export DJANGO_SETTINGS_MODULE=config.settings.production
```
O en cambio:
```bash
# Cambiar a desarrollo
export DJANGO_SETTINGS_MODULE=config.settings.development
```
Luego correr el servidor con:
```bash
python manage.py runserver
```

## Estructura del proyecto
```plaintext
├── api
├── apps
│   └── users
├── config
│   ├── asgi.py
│   ├── __init__.py
│   ├── __pycache__
│   ├── settings
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── db.sqlite3
├── manage.py
├── README.md
├── requirements.txt
```
## Diferencia entre apps/ y API/
Apps contiene toda la logia de negocio, por ejemplo:
```plaintext
apps/users/
├── models.py
├── services.py
├── repositories.py
└── selectors.py
```

APi cotiene todo lo relacionado a HTTP/REST, por ejemplo:
```plaintext
api/v1/users/
├── serializers.py
├── views.py
└── urls.py
```
