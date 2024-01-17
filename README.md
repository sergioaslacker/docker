# Docker 2024
En este repositorio estan consideradas las 2 pruebas definidas para Docker descritas a continuación y se irán agregando funcionalidades según definiciones y avances en las pruebas:
- Contenedor con MySQL
- Contenedor con phpmyadmin (bitnami)

####Referencias/Documentación de tecnología de componentes
- [Docker Hub: MySQL](https://hub.docker.com/_/mysql)
- [Docker Hub: phpmyadmin](https://hub.docker.com/r/bitnami/phpmyadmin)

## Instalación

Se requiere tener **Docker** y **Docker-Compose** instalados en el sistema

- [Docker Desktop en Windows](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe?utm_source=docker&utm_medium=webreferral&utm_campaign=dd-smartbutton&utm_location=module&_gl=1*11amgsu*_ga*MTA5MzUxMzYyNi4xNzA1NDMxOTYy*_ga_XJWPQMJYHQ*MTcwNTQ5ODIyNy4yLjEuMTcwNTUwMDM3MC41Mi4wLjA.)
- [Docker Desktop en Mac Intel Chip](https://desktop.docker.com/mac/main/amd64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=dd-smartbutton&utm_location=module&_gl=1*1qspo44*_ga*MTA5MzUxMzYyNi4xNzA1NDMxOTYy*_ga_XJWPQMJYHQ*MTcwNTQ5ODIyNy4yLjEuMTcwNTUwMDM3MC41Mi4wLjA.)
- [Docker Desktop en Mac Apple Chip](https://desktop.docker.com/mac/main/arm64/Docker.dmg?utm_source=docker&utm_medium=webreferral&utm_campaign=dd-smartbutton&utm_location=module&_gl=1*1qspo44*_ga*MTA5MzUxMzYyNi4xNzA1NDMxOTYy*_ga_XJWPQMJYHQ*MTcwNTQ5ODIyNy4yLjEuMTcwNTUwMDM3MC41Mi4wLjA.)
- [Docker Desktop en Linux](https://docs.docker.com/desktop/linux/install/?_gl=1*1qspo44*_ga*MTA5MzUxMzYyNi4xNzA1NDMxOTYy*_ga_XJWPQMJYHQ*MTcwNTQ5ODIyNy4yLjEuMTcwNTUwMDM3MC41Mi4wLjA.)

- [Docker Compose](https://docs.docker.com/compose/)

## Inicializar contenedores

Ambos contenedores están en las carpetas **mysql** y **phpmyadmin** respectivamente, en la carpeta raíz denominada **docker**

#### MySQL

```
docker
├── mysql
    └── docker-compose.yml
```

Acceder a la ruta *docker/mysql* y ejecutar el siguiente comando: 
```
docker-compose up
```

La base de datos queda disponible en el puerto 3306 y se accede con las siguientes credenciales:
```
NombreDB:       sqldb
User:           root
RootPassword:   dreamsql
```

#### PhpMyAdmin

```
docker
├── phpmyadmin
    └── docker-compose.yml
```

Acceder a la ruta *docker/phpmyadmin* y ejecutar el siguiente comando: 
```
docker-compose up
```

El administrador queda disponible en **localhost** y se accede con las siguientes credenciales:
```
User:           root
RootPassword:   bitnami
```