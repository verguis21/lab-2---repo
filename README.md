# Laboratorio 02
Hoy utilizaremos docker compose para poder desplegar su trabajo. Servicio web y una
base de datos

## Stack
API
    -Minimal API
        Debe retornar un mensaje incluyendo mi nombre
    - Docker
-docker run -d --rm -p 3000:3000 nmatsui/hello-world-api. 7ff11e1db7c2 great_benz
docker run -d --rm -p 3001:3000 nmatsui/hello-world-api  ab712e9fd260  hungry_robinson
docker run -d --rm -p 3002:3000 nmatsui/hello-world-api  4183e3e2c579  stoic_lehmann


BD
    - PostgreSQL
-$ docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d
postgres

# Indicaiones 

## Comandos

``` bash
docker compose up -d
```
## Configuracion del entorno 

```
MESSAGE=<Colocar nombre>
```

# Creditos
-Vegaray Colonia, José Francisco

#ETC
