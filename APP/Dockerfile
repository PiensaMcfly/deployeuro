# Usa una imagen base de OpenJDK 8
FROM openjdk:8-jdk-alpine

# Define el directorio de trabajo dentro del contenedor
WORKDIR /app

# Argumento que define el nombre del JAR
ARG JAR_FILE=target/AppEuro-0.0.1-SNAPSHOT.jar

# Copia el archivo JAR generado en el contenedor
COPY ${JAR_FILE} EuroSportAPP.jar

# Exponer el puerto 8080
EXPOSE 8080

# Comando para ejecutar la aplicación
ENTRYPOINT ["java", "-jar", "EuroSportAPP.jar"]
