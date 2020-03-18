ARG TAG=1.17-alpine

FROM nginx:$TAG

LABEL mantainer="mirko@altragamma.it"
LABEL description="NGINX Gateway Container"

# ADD data in image when build
ADD ./nginx.conf /etc/nginx/nginx.conf
ADD ./kibana.conf /etc/nginx/conf.d/kibana.conf