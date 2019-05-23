FROM java:8 
COPY target/App-jar-with-dependencies.jar App.jar
EXPOSE 4567
CMD ["/usr/lib/jvm/java-8-openjdk-amd64/bin/java", "-jar", "App.jar"]