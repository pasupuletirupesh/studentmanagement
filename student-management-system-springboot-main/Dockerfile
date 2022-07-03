#FROM maven
#COPY ./ ./
#RUN mvn clean package

FROM openjdk:11
VOLUME /tmp
EXPOSE 8080
ADD target/*.jar student.jar
ENV JAVA_OPTS=""
ENTRYPOINT ["java","-jar","target/student-management-system-0.0.1-SNAPSHOT.jar"]

#FROM openjdk:8-jdk-alpine
#VOLUME /tmp
#EXPOSE 8000
#ADD target/*.jar app.jar
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]