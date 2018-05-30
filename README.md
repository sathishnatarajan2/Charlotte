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
    
 
## How it works:
* Source code has checked in [Git Repositary](https://github.com/sathishnatarajan2/Charlotte.git)
* CI/CD Concourse Pipeline has configured with Git Repositary with timer of every two minutes it listens any update on the repo, accordingly it does the latest build and pushes the package into  [Pivotal.io PFS](https://run.pivotal.io/)
* Configured MySql Service available from Pivotal Marketplace

## Build the app with maven

```
$ mvn clean package
```

## Deploy the war to PCF

```
$ cf push Charlotte -p target/charlotte.war
```

# APP URL [https://charlotte-subpubescent-moonrise.cfapps.io/](https://charlotte-subpubescent-moonrise.cfapps.io/)
# CI /CD Pipeline: [http://192.168.99.100:8080/teams/main/pipelines/Charlotte](http://192.168.99.100:8080/teams/main/pipelines/Charlotte)


