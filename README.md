# docker_maven

docker run -it --rm --name my-maven-project -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven maven:3.3-jdk-8 mvn clean install

https://spring.io/guides/gs/maven/

cp /target/gs-maven-0.1.0.war /etc/tomcat/webapps/

#https://husbch.medium.com/mini-project-deploying-java-application-with-tomcat-bd7d96bfcc7
