![php](	https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![mysql](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![docker](	https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
![mariadb](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)

	

[![@sergioantoniobgz](https://img.shields.io/badge/@sergioantoniobgz%20%20-Sergio%20A.Slacker%20-black.svg?style=flat-square)](https://www.slackdistraught.com)

[npm-coreui-angular]:              https://www.npmjs.com/package/@coreui/angular
[npm-coreui-angular-badge]:        https://img.shields.io/npm/v/@coreui/angular.png?style=flat-square
[npm-coreui-angular-badge-latest]: https://img.shields.io/npm/v/@coreui/angular-pro/latest?style=flat-square&color=red
[npm-coreui-angular-badge-next]:   https://img.shields.io/npm/v/@coreui/angular-pro/next?style=flat-square&color=yellow
[npm-coreui-angular-download]:     https://img.shields.io/npm/dm/@coreui/angular.svg?style=flat-square
[npm-coreui]:                      https://www.npmjs.com/package/@coreui/coreui
[npm-coreui-badge]:                https://img.shields.io/npm/v/@coreui/coreui-pro.png?style=flat-square
[npm-coreui-download]:             https://img.shields.io/npm/dm/@coreui/coreui.svg?style=flat-square

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