FROM xeor/base-centos-daemon

MAINTAINER Lars Solberg <lars.solberg@gmail.com>
ENV REFRESHED_AT 2015-01-29

RUN yum install -y nginx inotify-tools

COPY init/ /init/
COPY supervisord.d/ /etc/supervisord.d/
COPY nginx.tmpl /
COPY nginx.conf /etc/nginx/nginx.conf
COPY generator.sh /

EXPOSE 80
EXPOSE 443
