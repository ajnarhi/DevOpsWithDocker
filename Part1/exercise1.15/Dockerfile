FROM openjdk:8
WORKDIR /myapp
COPY ot-harjoitustyo .
RUN apt-get update && apt-get install -y maven
WORKDIR /myapp/TuplakonsonantitJaVokaalit
RUN mvn package 

EXPOSE 8080
CMD ["java","-jar","target/TuplakonsonantitJaVokaalit-1.0-SNAPSHOT.jar"]
