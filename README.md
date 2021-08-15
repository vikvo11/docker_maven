# docker_maven

docker run -it --rm --name my-maven-project -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven maven:3.3-jdk-8 mvn clean install

https://spring.io/guides/gs/maven/

cp /target/gs-maven-0.1.0.war /etc/tomcat/webapps/

#https://husbch.medium.com/mini-project-deploying-java-application-with-tomcat-bd7d96bfcc7

###	If you’ve changed the value of <packaging> from "jar" to "war", the result will be a WAR file within the target directory instead of a JAR file.
  
mkdir -p src/main/webapp/WEB-INF/ 
  vim src/main/webapp/WEB-INF/web.xml
  
  <plugin>            
  <groupId>org.apache.maven.plugins</groupId>
  <artifactId>maven-war-plugin</artifactId>
  <configuration>
    <webXml>src\main\webapp\WEB-INF\web.xml</webXml>        
  </configuration>
</plugin>
