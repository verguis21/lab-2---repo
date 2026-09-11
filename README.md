# Laboratorio 02
Hoy utilizaremos docker compose para poder desplegar su trabajo. Servicio web y una
base de datos

## Stack
API
    - Minimal API
        Debe retornar un mensaje incluyendo mi nombre
    - Docker
- docker run -d --rm -p 3000:3000 nmatsui/hello-world-api. 7ff11e1db7c2 great_benz
- docker run -d --rm -p 3001:3000 nmatsui/hello-world-api  ab712e9fd260  hungry_robinson
- docker run -d --rm -p 3002:3000 nmatsui/hello-world-api  4183e3e2c579  stoic_lehmann


BD
    - PostgreSQL
-$ docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d
postgres

# Indicaciones 

## Comandos

``` bash
docker compose up -d
```
``` bash
docker compose down
```
``` bash
docker logs
```
``` bash
curl.exe -i http://localhost:3003/     
```
## Configuracion del entorno 

```
MESSAGE=<Colocar nombre>
```

# Creditos
-Vegaray Colonia, José Francisco

# PREGUNTAS
# TIPOS DE REDES
- **bridge:** Es la redpor defecto , funciona creando una red virtual privada interna en el host
- **HOST:** Elimina el aislamiento de la red 
- **OVERLAY:** Utilizada para conectar multiples dominios de docker entre si 
- **MACVLAN:** Asigna una direccion MAC unica al contenedor
- **NONE:** Deshabilita toda la conexion de red, aislando el contenedor por completo

# TIPOS DE VOLUMEN 
- **NAMED VOLUMES:** Son gestionados íntegramente por Docker (se almacenan en una ruta protegida).
- **BIND MOUNTS:** Mapean una ruta absoluta especifica de la maquina anfitriona directamente dentro del contenedor.
- **TMPFS MOUNTS:** Almacena los datos de forma temporal unicamente en la memoria RAM del host.