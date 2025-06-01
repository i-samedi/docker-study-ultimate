# docker cp    ID:DIRECCION-DEL-ARCHIVO     IRECCION-DONDE-COPIAR
=> del contenedor a la maquina

# docker cp 92de3a843142:/app/contenedor.txt .   
=> . : es en el directorio actual; ahi se copio

# docker cp anfitrion.txt 92de3a843142:/app/  
=> de la maquina al contenedor
=> /app $ cat anfitrion.txt : con CAT se puede ver lo que contiene