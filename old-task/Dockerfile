FROM frolvlad/alpine-oraclejdk8:slim
MAINTAINER "jeesun"<simon.sun.dev@hotmail.com>
VOLUME /tmp
ADD /target/old-task-*.jar app.jar
RUN sh -c "touch /app.jar"
ENV JAVA_OPTS=""
EXPOSE 8184
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
