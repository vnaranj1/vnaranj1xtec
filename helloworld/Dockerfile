# Utiliza la imagen oficial de nginx (servidor web) en su versión alpine (más ligera)
FROM nginx:alpine

# Crea un archivo index.html con el contenido "Hola Mundo"
RUN echo "<h1>Hola Mundo</h1>" > /usr/share/nginx/html/index.html

# Crea un directorio html-2
RUN mkdir  /usr/share/nginx/html-2

# Expone el puerto 8181
#EXPOSE 8181

# Configura el puerto en la configuración de nginx
#RUN sed -i 's/listen 80;/listen 8181;/g' /etc/nginx/conf.d/default.conf

# Inicia el servidor nginx
CMD ["nginx", "-g", "daemon off;"]
