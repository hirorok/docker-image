FROM alpine
LABEL maintainer="creater beginner"
RUN apk --no-cache update 
RUN apk --no-cache add openrc
RUN apk --no-cache add nginx
ADD index.html /www/index.html
ADD nginx.conf /etc/nginx/nginx.conf
RUN rc-update add nginx
