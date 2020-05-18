FROM docker.elastic.co/apm/apm-server:7.7.0
COPY config/apm-server.yml /usr/share/apm-server/apm-server.yml
#RUN chmod go-w /usr/share/apm-server/apm-server.yml
#USER root
#RUN chown root:apm-server /usr/share/apm-server/apm-server.yml
#USER apm-server

USER root
RUN chown apm-server /usr/share/apm-server/apm-server.yml && chmod go-w /usr/share/apm-server/apm-server.yml
USER apm-server
RUN cat /usr/share/apm-server/apm-server.yml