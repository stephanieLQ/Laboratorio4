# Instrucciones para ejecutar

### Requisitos
El docker-compose.yml del laboratorio 4 usa repositorios docker desde nexus, para lo cual se necesita los siguientes requisitos:

1. Iniciar el servidor nexus
```
$ docker compose up -d nexus
```
2. Configurar docker hosted en los repositorios nexus
3. Permitir acceso sin autenticación
4. Se debe generar la imagen del repositorio [frontend-docker](https://github.com/stephanieLQ/frontend-docker)
5. Se debe generar la imagen del repositorio [backen-docker](https://github.com/stephanieLQ/backend-docker)
6. Subirl la imagenes al servidor nexus.

### Orden de inicio de los servicios
1. Levantar servidor nexus
```
$ docker compose up -d nexus
```
2. Levantar servicio mongo
```
$ docker compose up -d mongo
```
3. Levantar servicio backend
```
$ docker compose up -d backend
```
4. Levantar servicio frontend
```
$ docker compose up -d frontend
```