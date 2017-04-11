FROM golang:alpine

MAINTAINER GuHao <378999587@qq.com>

ENV TZ "Asia/Shanghai"

ENV GOPATH /data/go
ENV PATH $GOPATH/bin:/usr/local/go/bin:$PATH

RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
WORKDIR /data

RUN go get github.com/num5/chca

COPY conf.ini /data/conf.ini

VOLUME ["./markdown","/data/markdown"]
VOLUME ["./theme","/data/theme"]

RUN chca init \
    & chca compile \
