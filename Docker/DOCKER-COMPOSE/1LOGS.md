# docker compose up --build -d
--build : asegurar imagenes siempre se crean desde cero y no ocupa una ya usada

ver log de contenedor
# docker compose logs
-f : para seguir logs
-t : ver timestamp

--until: para ver de q fechas a que fechas
--since: ambos para rangos de fechas

# docker compose ps
para ver todos con contenedores ejecutandose con docker compose

# docker compose down 
detiene y elimina 