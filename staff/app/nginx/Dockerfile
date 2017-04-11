FROM nginx:alpine

MAINTAINER GuHao <378999587@qq.com>

ENV TZ "Asia/Shanghai"

#COPY nginx.conf /etc/nginx/nginx.conf
COPY default.conf /etc/nginx/conf.d/default.conf

#VOLUME ["/data/docker/nginx/www","/usr/share/nginx/html"]
#VOLUME ["./logs","/var/log"]

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
