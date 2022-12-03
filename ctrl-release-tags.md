TAG v0.0.1.221202
Release:
Titulo: Creada la Base de Proyecto

## Base del Proyecto
- Contenedores de Python y PosgeSQL
- En el contenedor de Python, se instala Django.
- Se crean un programa para esperar que la DB se active y luego se levanta la APP.
  - Esto solo sucede si se trabaja con contenedores.
- Se configura GitHub para que trabaje con Docker, revisando que el código este bien escrito.
  - Con *Actions* de GitHub
- Levantar el proyecto si es la primera vez: `docker-compose build`
- Ya luego solamente con: `docker-compose up`
- Crear el super usuario:
  - `docker-compose run --rm app sh -c "python manage.py createsuperuser`
- Ya se a trabajado en la creación de usuarios para que pida solo correo y passwd.
- Tambien se ha trabaja do en la presentasión del _admin_.