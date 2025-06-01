>docker start

1. **docker create --help** : Para poder ver la documentación.
2. > docker create -[nombre de la imagen] : [etiqueta] : Crea un contenedor pero no lo ejecuta.
3. > docker ps -a : Para ver los contenedores creados pero no en ejecución.
4. > docker ps : Para ver contenedores ejecutados.

# docker create --name nombre nombreimagen:etiqueta

# docker start nombre
# docker stop "id del contenedor" o el nombre

o

# docker run --nombre imagenName:etiqueta
va a dejar la terminal tomada 
Si se sale Ctl+C se detiene
Pero si se hace lo siguiente:
# docker run -d --nombre imagenName:etiqueta
Al colocar -d tienes acceso a la terminal

# docker container prune
Elimina todos los contenedores

docker create app-react:3
docker ps -a #para ver los contenedores no ejecutados

docker run -d --name holala app-react:3  #sin la -d se va a acceder dentro del contenedor, y si se hace un ctl+c se detiene

docker container prune #elimina todos los contenedores que no estan ejecutados