# utilisation image nginx
FROM nginx:alpine

# copie des fichiers frontend
COPY . /usr/share/nginx/html

# expose le port http
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]