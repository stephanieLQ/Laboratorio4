# Laboratorio4
modulo8-lab4

Requisitos
El docker-compose.yml del laboratorio 4 usa repositorios docker desde nexus, para lo cual se necesita los siguientes requisitos:

Iniciar el servidor nexus
$ docker compose up -d nexus
Configurar docker hosted en los repositorios nexus
Permitir acceso sin autenticación
Se debe generar la imagen del repositorio frontend-docker
Se debe generar la imagen del repositorio backen-docker
Subirl la imagenes al servidor nexus.
Orden de inicio de los servicios
Levantar servidor nexus
$ docker compose up -d nexus
Levantar servicio mongo
$ docker compose up -d mongo
Levantar servicio backend
$ docker compose up -d backend
Levantar servicio frontend
$ docker compose up -d frontend