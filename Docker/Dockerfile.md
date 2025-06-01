>Instalar runtime, instalar dependencias, ejecutar proyecto.
>
>Por que se incluyen archivos???
>- Para tomar menos tiempo.
>- Para que las imagenes pesen menos, mas faciles de transferir por la red.

Código PLATO para empaquetar aplicaciones todo lo necesario como VERSIÓN Y AMBIENTE DE EJECUCIÓN.

> Un ***CONTENEDOR*** es un ***PROCESO***,
> Mientras que una ***APP*** es un ***CÓDIGO ALMACENADO***,
> Y el ***PROCESO*** es el ***CÓDIGO EJECUTANDOSE***.

- ***Contenedor = Proceso*** ... que procesa sistema de archivos
- ***Imagen = Aplicación***
#### ***! EL CONTENEDOR SE INICIA CUANDO LA IMAGEN ES EJECUTADA!!!!!***

## [Imagen](Iniciar_Imagen.md)
Una imagen es una aplicación que tiene todo lo necesario para ejecutarse, incluyendo el código, runtime, librerías, variables de entorno y archivos de configuración.

Dependencias (*nodejs, python, java, etc*) y el Sistema Operativo.

## [Contenedor](Iniciar_Contenedores.md)
Es un proceso, inicia a partir de una imagen con su propio sistema de archivos, ambiente aislado.
Puede detenerse y volver a iniciar.

- **Puede haber MULTIPLES CONTENEDORES a través de la misma imagen !!!!**
#### OJO !!!
Contenedores independientes PERO se pueden comunicar!
CADA CONTENEDOR ES SU PROPIO UNIVERSO...
- SI ***A*** se *MODIFICA*, *NO* *INTERFIERE* a ***B*** 