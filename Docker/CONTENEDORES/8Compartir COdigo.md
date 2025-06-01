# volumenes anonimos = no se le indica nombre
sino directorio por ejemplo
# docker run -d -p 80:5173 --name NAME -v ./:/app/datos IMAGEN:TAG
=> se vincula todo el proyecto
-> no sirve para distintos OS

# docker run -d -p 80:5173 --name holala -v ./src:/app/src  app-react:4 
=> puede verse todas las actualizaciones del area de desarrollo
    ya que no se esta trabajando con COPIAS