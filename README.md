## SWARM CON SERVICIOS SOAP Y REST

## PASO 1 Crear las imagenes

## en apiRest
`docker build . -t restapi`
## en apiSoap
`docker build . -t soapapi`
## en client
`docker build . -t client`
## en mysql
`docker build . -t mysql`

## PASO 2 Desplegar los servicios con swarm

`docker swarm init`

`docker stack deploy -c docker-compose.yml mis-servicios`

## Aclaraciones

Se creo el servidor SOAP en el puerto 4000

El servidor web se encuentra alojado en localhost:8080