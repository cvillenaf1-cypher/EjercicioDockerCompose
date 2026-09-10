# Laboratio 02 - docker compose
Trabajar un docker compose, especificando configuración y comandos para despliegue. Debe permitir lo siguiente:




 ## ASIGNACIÓN EN DOCKER  COMPOSE
 para  contrucción de las copias:
```bash
 build: ./api
 ````
 - api1: puerto 3000
 - api2: puerto 3001
 - api3: puerto 3002


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