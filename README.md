# Laboratio 02 - docker compose
Trabajar un docker compose, especificando configuración y comandos para despliegue. Debe permitir lo siguiente:

trabajo de manera manual 
- imagen utilizada: docker pull nmatsui/hello-world-api + ejecucion
para ejecutar las copias :
docker run -d --rm -p 3000:3000 nmatsui/hello-world-api , luego cambiamos el puerto al  3001 y 3002 para los respectivos contenedores
-copia 1 en  el puerto 3000 : nifty_bose
-copia 2 en el puerto 3001 : interesting_rubi
-copia 3 en el puerto 3002: sleepy_raman
 asiganacion en compose  
 api1: puerto 3000
 api2: puerto 3001
 api3: puerto 3002