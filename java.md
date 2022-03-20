# Important Commands: Java MVN
---

Install external jars
```
mvn install:install-file -Dfile=<jar-location> -DgroupId=<groupId> -DartifactId=<artifact> -Dversion=<version> -Dpackageing=<packaging>
mvn install:install-file -Dfile=<D:\jar\dns.jar> -DgroupId=org.xbill -DartifactId=dns -Dversion=2.0.8 -Dpackageing=jar
```

Run MVN clean install
```
mvn clean install -Dspring.profiles.active=<profile> -Dmaven.test.skip=true
mvn clean install -Dspring.profiles.active=local -Dmaven.test.skip=true
```

Run Maven Test Cases
```
mvn test -Dspring.profiles.active=<profile> 
mvn clean test -Dspring.profiles.active=local
```

Springboot Run
```
mvn spring-boot:run -Dspring.profiles.active=<profile> -Dmaven.test.skip=true
mvn spring-boot:run -Dspring.profiles.active=local -Dmaven.test.skip=true
```

Run Jar file
```
java -jar <jar-name>
java -jar appname-0.0.1-SNAPSHOT.jar
```
