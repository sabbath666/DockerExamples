FROM openjdk:21
WORKDIR /app
COPY ./settings.yml /app/settings.yml
COPY target/cowsay-0.0.1.jar cowsay.jar
RUN mkdir data
ENTRYPOINT ["java", "-jar", "cowsay.jar"]