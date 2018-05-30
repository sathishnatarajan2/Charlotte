# This is the Modernization POC Project to be deployed in Pivotal Cloud Foundry Platform
* Website: [concourse-ci.org](https://concourse-ci.org)
* `Technology Stack`:
  * [About](https://concourse-ci.org/about.html)
  * [Setting Up](https://concourse-ci.org/install.html)
  * [Using Concourse / Docs](https://concourse-ci.org/)
* Forum 
  * [Concourse Discourse](https://discuss.concourse-ci.org)
* Chat
  * [Discord](https://discord.gg/MeRxXKW)
* Roadmap:
  * [GitHub Milestones](https://github.com/concourse/concourse/milestones)
  * [GitHub Issues](https://github.com/concourse/concourse/issues)

 `*Technology Stack`
    * Deployment environment [Pivotal.io PFS] (https://run.pivotal.io/)
    * Development Framework: Spring 4.4, Spring Cloud Services,
    * Database: MYSQL Service
    * Database connectivity driver: JPA
    * Build Pack : Java
    * Build Tool: Maven
    * Java version JDK 1.8
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


