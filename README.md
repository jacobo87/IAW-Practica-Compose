# IAW - Práctica 15
>IES Celia Viñas (Almería) - Curso 2020/2021   
>Módulo: IAW - Implantación de Aplicaciones Web   
>Ciclo: CFGS Administración de Sistemas Informáticos en Red 

# Contenido
Realizar la implantación de un sitio WordPress en Amazon Web Services (AWS) haciendo uso de contenedores Docker y la herramienta Docker Compose.

Los servicios definidos en el archivo docker-compose.yml deberán usar dos redes:
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
