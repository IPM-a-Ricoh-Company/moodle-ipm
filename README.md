# moodle-ipm

## Descripción
Repositorio dedicado a la aplicación moodle basada en contenedores lista para desplegar mediante kustomization
Se compone de las siguientes partes:
- Moodle en versión 4.3
- Base de datos MySQL replicada versión 8.3
- Base de datos de cache REDIS replicada versión 6.2

## Componentes principales de cada elemento
###Moodle
- Acceso por servicio balanceado de capa4 (IP)
- Almacenamiento persistente en vSAN File Services
- Despliegue en alta disponibilidad (3 pods) en nodepool propio

###BBDD MySQL
- Base de datos replicada
- Accceso mediante servicio balanceado capa4 (IP)
- Almacenamiento persistente en vSAN File Services
- Replicación mediante nodo primario y nodo secundario

###REDIS
- Base de datos replicada
- Accceso mediante servicio balanceado capa4 (IP)
- Almacenamiento persistente en vSAN File Services
- Replicación mediante nodo master y nodo replica
