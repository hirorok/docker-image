FROM alpine
LABEL maintainer="creater beginner"
RUN apk --no-cache add openrc nginx
RUN adduser -D -g 'www' www
RUN chown -R www:www /var/lib/nginx
ADD index.html /www/index.html
ADD nginx.conf /etc/nginx/nginx.conf
RUN chown -R www:www /www
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
