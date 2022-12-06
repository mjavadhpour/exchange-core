FROM eclipse-temurin:8-alpine as jdk

WORKDIR /opt/app

# Install JAVA 17 for vscode
COPY --from=eclipse-temurin:17-alpine $JAVA_HOME $JAVA_HOME/../openjdk17
ENV JDK_HOME="$JAVA_HOME/../openjdk17"

# Install Maven
COPY --from=maven:3-eclipse-temurin-8-alpine /usr/share/maven /usr/share/maven
RUN \
  ln -s /usr/share/maven/bin/mvn /usr/bin/mvn

CMD ["sleep", "infinity"]