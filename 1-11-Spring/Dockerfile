FROM openjdk:8

EXPOSE 3000

COPY . .

RUN ./mvnw package

CMD ["java","-jar","./target/docker-example-1.1.3.jar"]
