FROM alpine
LABEL maintainer="creater beginner"
RUN apk --no-cache add openrc nginx
RUN adduser -D -g 'www' www
ADD index.html /www/index.html
ADD nginx.conf /etc/nginx/nginx.conf
CMD [ "/usr/sbin/nginx","-c /etc/nginx/nginx.conf" ] 
