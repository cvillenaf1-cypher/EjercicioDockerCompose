# Laboratio 02 - docker compose
Trabajar un docker compose, especificando configuración y comandos para despliegue. Debe permitir lo siguiente:

## trabajo de manera manual 
- imagen utilizada: docker pull nmatsui/hello-world-api + ejecucion
para ejecutar las copias :
docker run -d --rm -p 3000:3000 nmatsui/hello-world-api , luego cambiamos el puerto al  3001 y 3002 para los respectivos contenedores
-copia 1 en  el puerto 3000 : nifty_bose
-copia 2 en el puerto 3001 : interesting_rubi
-copia 3 en el puerto 3002: sleepy_raman

## PARA SEGUIR  ELIMINO ESTOS CONTENEDORES PARA TENER LOS PUERTOS LIBRES

 ASIGNACIÓN EN DOCKER  COMPOSE
 api1: puerto 3000
 api2: puerto 3001
 api3: puerto 3002


### Tipos de Redes en Docker

Bridge: Crea una red privada e interna dentro del host, permitiendo que los contenedores aislen el trafico exterior.

Host: Elimina el aislamiento Y el contenedor usa la red del sistema anfitrión.

Overlay: Conecta múltiples servidores físicos en clústeres mediante Docker Swarm.

Macvlan: Asigna una dirección MAC física al contenedor en la red local.

None: Desactiva toda la conectividad de red del contenedor.


 ### Tipos de Volúmenes en Docker

Volumes: Almacenamiento persistente administrado directamente por Docker.

Bind Mounts: Vincula directamente una ruta física de la máquina host al contenedor.

tmpfs Mounts: Almacena datos temporalmente en la memoria RAM del host. 

