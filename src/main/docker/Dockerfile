FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD sfg-thymeleaf-course-1.1.jar scbApp.jar
RUN sh -c 'touch scbApp.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar scbApp.jar" ]
