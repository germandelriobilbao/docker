FROM alpine:latest
LABEL maintainer="Germán del Río Bilbao <german.d.rio.bilbao@accenture.com>"

RUN apk --no-cache add openjdk11 --repository=http://dl-cdn.alpinelinux.org/alpine/edge/community
RUN mkdir /apps
WORKDIR /apps
RUN wget http://apache.uvigo.es//jmeter/binaries/apache-jmeter-5.2.1.tgz
RUN tar -zxvf apache-jmeter-5.2.1.tgz
RUN rm -f apache-jmeter-5.2.1.tgz

RUN chmod 777 -R /apps

CMD tail -f /dev/null
