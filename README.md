# Mi Primer Dockerfile 

presentacion [link](https://docs.google.com/presentation/d/17Xpk3lviU3tv_ecHKrxjkYY76PQ2ijdswcZd7dJh07s/edit?usp=sharing)

conjuntos de ejemplos de como empezar a usar docker.

comandos utiles

build 
```
docker build -t "namecontainer" .
```
revisar contenedores corriendo
```
docker ps 
```
revisar todos los contenedores aun los que estan detenidos
```
docker ps -a
```
listar volumenes
```
docker volume ls 
```

arrancar o correr
```
docker run
```
detener
```
docker stop "contenedornombre/ o ID"
```


## ejemplo1

ejemplo de web server Apache

construir primer contenedor
```
docker build -t ejemplo1 .
```
levantar contenedor 
```
docker run  -p 8080:80 ejemplo1
```
montar carpeta customizada
```
docker run -p 8080:80 -v "rutalocal:rutacontenedor" ejemplo1
```

```
 docker run -p 8080:80 -v $PWD/testlive/:/var/www/html/ ejemplo1 
```


## ejemplo2

node js skeleton app

build
```
docker build -t ejemplo2 .
```

run 
```
docker run -p 8080:8080 ejemplo2
```


## ejemplo 3

construir 
```
docker build -t ejemplo3 .

```

correr contenedor 
```
docker run -p 8000:5000 ejemplo3

```

## ejemplo 4

construir 
```
docker build -t ejemplo4 .

```

correr contenedor 
```
docker run -p 8000:5000 ejemplo4

```

# Recursos


https://docs.docker.com/install/
https://labs.play-with-docker.com/
https://docker-curriculum.com/

