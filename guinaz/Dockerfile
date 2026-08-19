FROM nginx:alpine

COPY index.html products.html support.html /usr/share/nginx/html/
COPY css /usr/share/nginx/html/css/
COPY nginx.conf /etc/nginx/nginx.conf

RUN chown -R nginx:nginx /usr/share/nginx/html

USER nginx

EXPOSE 8080

ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]
