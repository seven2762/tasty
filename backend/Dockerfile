FROM eclipse-temurin:21
WORKDIR /app
RUN apt-get update && apt-get install -y dos2unix
COPY gradlew .
RUN dos2unix gradlew
CMD ["./gradlew", "bootRun", "-Dspring.profiles.active=dev"]