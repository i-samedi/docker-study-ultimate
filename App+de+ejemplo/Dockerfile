# FROM indicar imagen base y ser siempre especifico o afecta el comportamiento de la imagen
# WORKDIR cambiar el directorio de trabajo
# COPY ES MAS ESPECIFICO QUE ADD, SOLO COPIA ARCHIVOS LOCALES
# ADD PARA PODER AGREFAR ARCHIVOS IGUAL QUE COPY
# RUN ejecutar comandos (CUANDO SE CONSTRUYEN LAS IMAGENES)
# ENV variables de entorno
# EXPOSE exponer puertos de la aplicacion
# USER asignar usuarios con provilegios acotados
# CMD comando que se ejecuta al iniciar el contenedor (CUANDO SE EJECUTA EL CONTENEDOR)
# ENTRYPOINT comando que se ejecuta al iniciar el contenedor, se puede reescribir en la linea de comando.

# FROM node:20.5.0-alpine3.18
# WORKDIR /app/
# COPY . .
# # COPY ["package.json", "package-lock.json*", "./"]
# # ADD http://www.miweb.com/archivo.txt .
# # ADD archivo.zip .

# #comandos RUN
# RUN npm install

# # optimizar la construccion de imagenes
# # cada una es uma capa, reutilizar la misma capa que docker ya utilizo para que no se 
# # genere una nueva capa
# # COPY eliminara todas las capas hacia abajo y las va a recontruir desde cero!!!
# # las dependencias se deben de instalar todas devuevo pero!!!!!!

# # primero se copian las especificaciones de nuestras dependencias 
# COPY package*.json . 
# RUN npm install
# # y despues se van a copiar los archivos del proyecto
# COPY . .


# FROM node:20.5.0-alpine3.18
# WORKDIR /app/
# COPY package*.json . 
# RUN npm install
# COPY . .
# ENV API=https://api.mercadolibre.com
# EXPOSE 5173
# RUN addgroup react && adduser -S -G react react
# USER react
# # este puerto va a ser expuesto en el contenedor, no va a exponer el puerto en la maquina host
# CMD ["npm", "run", "dev"]
# ENTRYPOINT ["npm", "run", "dev"]
# CMD ES FACIL DE REEMPLAZAR
# ENTRYPOINT ES MAS DIFICIL DE REEMPLAZAR -> --entrypoint="otro comando"



FROM node:20.5.0-alpine3.18
RUN addgroup react && adduser -S -G react react
USER react
WORKDIR /app/
RUN mkdir datos
COPY --chown=react package*.json . 
RUN npm install
COPY --chown=react . .
ENV API=https://api.mercadolibre.com
EXPOSE 5173
CMD ["npm", "run", "dev"]


# forma de etiquetar: SEMVER, INCREMENTALES, LATEST, POR CODIGO
# LO IMPORTANTE ES QUE EL EQUIPO TENGA CLARO EL TIPO
#       docker build -t app-react:icycoffee .
#       docker build -t app-react:3.2.4 .
#       docker build -t app-react:1 .

# Para no crearla y MODIFICARLA:
#       docker image tag app-react:icycoffee app-react:2         