#  es muy pequeña esta version
FROM node:alpine
COPY . /app
WORKDIR /app
CMD node app.js

# docker build -t panorama .    # construir la imagen
# docker run panorama            # ejecutar la imagen
# docker run -p 3000:3000 panorama  # ejecutar la imagen y mapear el puerto 3000
# docekr image ls                # listar las imagenes