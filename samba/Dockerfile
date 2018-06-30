FROM alpine
LABEL maintainer="creater beginner"
RUN apk --no-cache add samba openrc
RUN adduser -D -g 'samba' samba
ADD ./smb.conf /etc/samba/smb.conf
CMD ["/bin/sh", "-c", "nmbd -D && smbd -F </dev/null"]