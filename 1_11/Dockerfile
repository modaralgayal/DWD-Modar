FROM amazoncorretto:8-alpine3.12-jdk


## I looked at a stack overflow example of a dockerfile, 
## it reminded me that i needed to 
## COPY the files in order to use them. 
COPY . .

RUN ./mvnw package

EXPOSE 3000

CMD [ "java", "-jar", "./target/docker-example-1.1.3.jar" ]