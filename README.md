# This is the Modernization POC Project deployed in Pivotal Cloud Foundry Platform
* `Technology Stack`:
  * Deployment environment [Pivotal.io PFS] (https://run.pivotal.io/)
  * Development Framework: Spring 4.4, Spring Cloud Services
  * Database: MYSQL Service
  * Database connectivity driver: JPA
  * Build Pack : Java 1.8
  * Build Tool: Maven
  * App container Library: Tomcat Embedded Server (TomEE)
  * Container service : Docker
  * Container Service Orchestration: Docker Machine, Docker Swarm
  * Continuous Integration: Concourse
    
 

## Build the app with maven

```
$ mvn clean package
```

## Deploy the war to PCF

```
$ cf push Charlotte -p target/charlotte.war
```

# APP URL [https://charlotte-subpubescent-moonrise.cfapps.io/](https://charlotte-subpubescent-moonrise.cfapps.io/)


