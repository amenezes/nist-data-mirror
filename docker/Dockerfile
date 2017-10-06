FROM maven:alpine

WORKDIR /app

COPY . .

RUN mvn clean package \
  && mkdir /data

CMD java -jar /app/target/nist-data-mirror.jar /data
