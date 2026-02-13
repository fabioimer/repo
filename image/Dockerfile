FROM nginx:alpine

ARG FQDN

COPY template.html /tmp/template.html

RUN sed "s/{{FQDN}}/${FQDN}/g" /tmp/template.html > /usr/share/nginx/html/index.html

EXPOSE 80

