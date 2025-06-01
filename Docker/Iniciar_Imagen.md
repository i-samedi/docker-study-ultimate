# docker build -t panorama 
construir la imagen
# docker run panorama 
ejecutar la imagen
# docker run -p 3000:3000 panorama 
ejecutar la imagen y mapear el puerto 3000
# docekr image ls 
listar las imagenes

forma de etiquetar: **SEMVER, INCREMENTALES, LATEST, POR CODIGO**
!!!! LO IMPORTANTE ES QUE EL EQUIPO TENGA CLARO EL TIPO
# docker build -t app-react:icycoffee .
Lo que esta despues de los dos puntos es la etiqueta que el equipo debe de tener claro.
# docker build -t app-react:3.2.4 .

# docker build -t app-react:1 .

# docker image tag app-react:icycoffee app-react:2
  Para no crearla y MODIFICARLA:     icycoffee -> 2