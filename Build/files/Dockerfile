FROM maven:alpine
RUN apk update &&\
    apk add git
WORKDIR /home/build
RUN mvn package
ENTRYPOINT cp target/*.war /tmp/ROOT.war