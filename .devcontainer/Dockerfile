FROM eclipse-temurin:19-alpine as jdk

WORKDIR /opt/app

COPY --from=eclipse-temurin:8-alpine $JAVA_HOME $JAVA_HOME/../openjdk8

CMD ["sleep", "infinity"]
