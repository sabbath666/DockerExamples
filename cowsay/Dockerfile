FROM maven:21 as build
COPY src /src
RUN mvn clean package

FROM build
WORKDIR /app
COPY target/cowsay-0.0.1.jar cowsay.jar
RUN mkdir data
ENTRYPOINT ["java", "-jar", "cowsay.jar"]