# Laboratio 02 - docker compose
Trabajar un docker compose, especificando configuración y comandos para despliegue. Debe permitir lo siguiente:




 ## ASIGNACIÓN EN DOCKER  COMPOSE
 para  contrucción de las copias:
```bash
 docker compose up -d --build
 ```
 - api1: puerto 3000
 - api2: puerto 3001
 - api3: puerto 3002

 para  verificar estado:
```bash
 docker compose ps
 ```

 para  detener la infraestructura:
```bash
 docker compose down
 ```
## Variables de entorno
- POSTGRES_USER=USER
- POSTGRES_CONTRA=CLAVE
- POSTGRES_DB=MYBASE
- NOMBRE= CRISTHIAN VILLENA

## Configuracion de bd
   - image: postgres:13  
    - container_name: postgres_db 
      - environment:
      - POSTGRES_USER: ${POSTGRES_USER}
      - POSTGRES_PASSWORD: ${POSTGRES_CONTRA}
      - POSTGRES_DB: ${POSTGRES_DB}



### Tipos de Redes en Docker

- Bridge: Crea una red privada e interna dentro del host, permitiendo que los contenedores aislen el trafico exterior.

- Host: Elimina el aislamiento Y el contenedor usa la red del sistema anfitrión.

- Overlay: Conecta múltiples servidores físicos en clústeres mediante Docker Swarm.

- Macvlan: Asigna una dirección MAC física al contenedor en la red local.

- None: Desactiva toda la conectividad de red del contenedor.


 ### Tipos de Volúmenes en Docker

- Volumes: Almacenamiento persistente administrado directamente por Docker.

- Bind Mounts: Vincula directamente una ruta física de la máquina host al contenedor.

- tmpfs Mounts: Almacena datos temporalmente en la memoria RAM del host. 

## Definimos volumen

- Nombre del volumen: postgres_data
- Driver: local
- Punto de montaje /var/lib/postgresql/data

## Comandos de Git
- coloca en zona de espera a los archivoa como por ejemplo para README:
```bash
 git add README.md
 ```

 - Crea un checkpoint + descripcion que facilita identificar el tipo de actualizacion  segun formato docs:, feat:, fix:

 ```bash
git commit -m "docs: modificacion de texo"
 ```
 - Aqui ya se sube a github

  ```bash
git push origin main
 ```