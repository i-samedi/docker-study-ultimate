# docker network ls
lista todas las redes de nuestra maquina con docker

Hay 3 redes que se crean por defecto: info respecto a sus DRIVER
    1. Bridge : red contenedores exclusivamente de esta red, se comunicaran entre si sin problema
    2. host : dejamos utilizar implementacion de docker, y se expondra y utilizar el puerto del SO del alfitrion
    3. none : driver de null: maquina que se encuentra dentro de esta red no se puede comunicar con nadie

    4. tambien esta Overlay: dos o mas maquinas ejecutando docker se puede ejecutar en red, se usa cuando despliega con KUBERNETES


al estar al mismo servicio se pueden comunicar y ver y hacer peticiones
pueden acceder directamente ya que estan en la misma red en este caso del yml es BRIDGE

# docker exec -it -u root 565 sh
## ping api 
realiza conexion y se ve la ip con: ifconfig !!!! solo se escribe el nombre d ela maquina
nunca se utiliza la IP

