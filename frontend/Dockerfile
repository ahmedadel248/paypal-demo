FROM alpine:3.18
RUN apk add nginx
COPY html/index.html /var/lib/nginx/html/index.html
COPY default.conf /etc/nginx/http.d/default.conf
EXPOSE 80
CMD ["nginx","-g","daemon off;"]