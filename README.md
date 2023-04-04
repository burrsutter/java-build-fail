# Java, Quarkus, Hello, with Dockerfile

### Build Failure Demo

The following commands only work if you fix the syntax error left in place purposefully for demo purposes

```
mvn package

java -jar target/java-build-fail-1.0.0-SNAPSHOT-runner.jar

curl localhost:8080

Hello Quarkus 4 12-23-2022 03:13:59 on unknown
```

```
docker build -f src/main/docker/Dockerfile.jvm -t java-build-fail .

docker run -i --rm -p 8080:8080 java-build-fail

curl localhost:8080

Hello Quarkus 1 12-24-2022 03:39:03 on e29c6975f9e3
```