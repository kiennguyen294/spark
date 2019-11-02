#FROM openjdk:8-jre-alpine
FROM goyalzz/ubuntu-java-8-maven-docker-image
RUN apt install git
#RUN apt install maven
RUN mkdir -p /opt/spark
WORKDIR /opt/spark
RUN git clone https://github.com/kiennguyen294/spark.git
WORKDIR /opt/spark/spark/spark-streaming-test
RUN mvn package
#COPY target/spark-streaming-test-1.0-SNAPSHOT-jar-with-dependencies.jar /app.jar
#CMD ["/usr/bin/java", "-jar", "/app.jar"]
