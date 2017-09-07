FROM openjdk
 
RUN mkdir -p /usr/local/demo
COPY target/spring-boot-rest-example-0.4.0.war /usr/local/demo/
VOLUME /tmp
ENV JAVA_OPTS="-Dspring.profiles.active=test"
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -jar /usr/local/demo/spring-boot-rest-example-0.4.0.war" ]
