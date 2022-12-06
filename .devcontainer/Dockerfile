FROM eclipse-temurin:19-alpine as jdk

WORKDIR /opt/app

# Install JAVA 8
COPY --from=eclipse-temurin:8-alpine $JAVA_HOME $JAVA_HOME/../openjdk8

# Install Maven
COPY --from=maven:3-eclipse-temurin-8-alpine /usr/share/maven /usr/share/maven
RUN \
  ln -s /usr/share/maven/bin/mvn /usr/bin/mvn

CMD ["sleep", "infinity"]
