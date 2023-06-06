# Usa una imagen base de Nginx
FROM nginx

# Copia los archivos de configuración de Nginx al contenedor
COPY nginx.conf /etc/nginx/nginx.conf

# Expone el puerto 80 para permitir conexiones externas
EXPOSE 80

# Crea un directorio para compartir archivos entre tu computadora y el contenedor
RUN mkdir /shared

# Configura los permisos del directorio compartido
RUN chmod 777 /shared

# Define el comando de inicio para el contenedor
CMD ["nginx", "-g", "daemon off;"]
