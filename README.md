# Epet
Game Epet

### 1. Crear el Proyecto Django

Si aún no has creado el proyecto Django, puedes hacerlo ahora desde dentro del contenedor. Primero, ejecuta el contenedor de manera interactiva:

```bash
docker-compose run web bash
```

Luego, dentro del contenedor, crea el proyecto Django (reemplaza `myproject` con el nombre que desees para tu proyecto):

```bash
django-admin startproject myproject .
```

### 2. Migraciones y Superusuario

Todavía dentro del contenedor, navega al directorio de tu proyecto Django si es necesario, y ejecuta las migraciones iniciales:

```bash
python manage.py migrate
```

También puedes crear un superusuario para acceder al admin de Django:

```bash
python manage.py createsuperuser
```

Sigue las instrucciones en pantalla para completar la creación del superusuario.

### 3. Acceder a tu Aplicación

Una vez que tu contenedor esté en funcionamiento, podrás acceder a tu aplicación Django desde tu navegador web visitando `http://localhost:8000`.
