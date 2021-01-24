# IAW - Práctica 15
>IES Celia Viñas (Almería) - Curso 2020/2021   
>Módulo: IAW - Implantación de Aplicaciones Web   
>Ciclo: CFGS Administración de Sistemas Informáticos en Red 

## Contenido
Realizar la implantación de un sitio WordPress en Amazon Web Services (AWS) haciendo uso de contenedores Docker y la herramienta Docker Compose.

## Instalación de WordPress usando contenedores Docker y Docker Compose

Tareas que tendrá que realizar:

- Crear una máquina virtual [Amazon EC2](https://aws.amazon.com/es/ "Amazon EC2").

- Instalar y configurar [Docker](https://www.docker.com/ "Docker") y [Docker compose](https://docs.docker.com/compose/ "Docker compose") en la máquina virtual.

- Crear un archivo `docker-compose.yml` para poder desplegar los servicios de **WordPress**, **MySQL** y **phpMyAdmin**. Deberá utilizar las imágenes oficiales de [Docker Hub](https://hub.docker.com/ "Docker Hub").

- Buscar cuál es la **dirección IP pública** de su instancia en **AWS** y comprobar que puede acceder a los servicios de **WordPress** y **phpMyAdmin** desde una navegador web.

------------

Los servicios definidos en el archivo `docker-compose.yml` deberán usar dos redes:
- frontend-network
- backend-network

En la red frontend-network estarán los servicios:
- WordPress
- phpMyAdmin

Y en la red backend-network sólo estará el servicio:
- MySQL

Sólo los servicios que están en la red frontend-network expondrán sus puertos en el host. Por lo tanto, el servicio de MySQL no deberá estar accesible desde el host.

## :warning:Importante:warning:
- Abrir todo el tráfico en la instancia.

## REFERENCIAS
- [José Juan Sánchez IAW - Práctica 15 ](https://josejuansanchez.org/iaw/practica-15/index.html)
- [Jacobo Azmani - Repositorio Docker-Compose](https://github.com/jacobo87/IAW-Practica-Compose)
