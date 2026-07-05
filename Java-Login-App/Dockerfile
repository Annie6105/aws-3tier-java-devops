FROM eclipse-temurin:11-jre

WORKDIR /app

COPY target/*.war app.war

EXPOSE 8080

ENTRYPOINT ["java","-jar","app.war"]