al tener dos contenedores
un archivo tiene y el otro no

# para guardar datos se deben de guardar en volumenes
host => CONTENEDOR
un volumen dentro del mismo host

o un link de un servicio etc

# docker volume create NAME
=> se crea el volumen
# docker volume inspect NAME
=> inspeccionar el volumen

# docker run -d -p 3000:3000 -v NAME:RUTA (/app/datos) IMAGEN:TAG
=> el volumen se guarda dentro de un directorio de un usuario root

se modifica en el archivo dockerfile:
# RUN mkdir datos
=> para que no sea usuario ROOT