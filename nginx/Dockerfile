FROM nginx

RUN rm -rf /etc/nginx/conf.d/default.conf
RUN rm -rf /etc/nginx/nginx.conf
RUN mkdir /etc/nginx/sites-enabled

ADD default.conf /etc/nginx/conf.d/
ADD nginx.conf /etc/nginx/
ADD gin.conf /etc/nginx/sites-enabled/
#ADD tonic.conf /etc/nginx/sites-enabled/

CMD ["nginx", "-g", "daemon off;"]
