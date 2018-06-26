From alpine
Label maintainer="creater beginner"
Run apk --no-cache update 
RUN apk --no-cache add openrc
RUN apk --no-cache add nginx
RUN rc-update add nginx
RUN rc-service nginx start
