# Arquitectura

Propuestas de cara a implementar una plantilla para la instalación del entorno de desarrollo remoto.
..........................................................
#Instalación minima en la maquina necesitara:

	Docker
	sshd
	git

#Aplicaciones a instalar para el desarrollo
	maven
	openjkd-7-jdk
	
#Instalacion de eclipse-che:

http://docs.codenvy.com/che/install/

#Eclipse-che Precompilado

http://docs.codenvy.com/download/#eclipse-che-binaries
	
#Instalacion de servicios:

	postgresql
	postgis
	geoserver
	
#Proyecto centa-redes y sus modulos:	
	centa-adasa/
	centa-adasa/postgis-spring-batch
	centa-adasa/postgis-spring-integration
	centa-adasa/postgis-spring-loader
	
	centa-adasa/oauth2-spring-server
	centa-adasa/oauth2-spring-service
	
	
	
..........................................................	
#Instalacion de Docker en Ubuntu:

```
$ sudo apt-get update
$ sudo apt-get install docker.io
$ source /etc/bash_completion.d/docker.io

# Instalacion sin apt
$ curl -sSL https://get.docker.com/ubuntu/ | sudo sh
```


#Vincular una cuenta GitHub con DockerHub:

https://registry.hub.docker.com/builds/link/github/

#Asociar un proyecto de github con docker para que se haga un despliegue automatico:

https://registry.hub.docker.com/builds/github/select/

#Vinculacion de un proyecto GitHub que contenga submodulos


#Remote Build triggers

Para lanzar el despliegue de un Dockfile lamando a la AIP REST por  HTTP:

http://docs.docker.com/docker-hub/builds/#remote-build-triggers

```
export PROJECT_KEY  = “”
export USUARIO = "illan"
export WEBHOOK = "buildhook"
curl --data "build=true" -X POST https://registry.hub.docker.com/u/${USUARIO}/${WEBHOOK}/trigger/${PROJECT_KEY}
```


```
sudo docker images
```


