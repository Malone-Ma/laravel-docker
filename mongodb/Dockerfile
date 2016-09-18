FROM mongo:latest

MAINTAINER Starriv <starriv.993@gmail.com>

COPY ./conf/mongod.conf /usr/local/etc/mongo/mongo.conf

VOLUME /data/db /data/configdb

# option "--rest","--httpinterface"
CMD ["mongod","-f","/usr/local/etc/mongo/mongo.conf"]


EXPOSE 27017 28017
