## Bonjour 👋

#### 🙋‍♀️ What is this? &rarr; an org used for microservies project.

Current services are developed using: `Java, Spring Boot, Eureka, Feign`

| Services | Detail | Port |
|----------|--------|------|
| [🐵 abomination-base](https://github.com/VL037-twittur/abomination-base) | base models maven dependency | |
| [🐶 twittur-db-migration](https://github.com/VL037-twittur/twittur-db-migration) | db migration | |
| [🐺 basilisk-registry](https://github.com/VL037-twittur/basilisk-registry) | eureka service registry | [:8761](http://localhost:8761) |
| [🐱 centaur-gateway](https://github.com/VL037-twittur/centaur-gateway) | api gateway | [:8080](http://localhost:8080) |
| [🦁 cyclops-account-credential](https://github.com/VL037-twittur/cyclops-account-credential) | account-credential service | [:8000](http://localhost:8000) |
| [🐯 gargoyle-account-profile](https://github.com/VL037-twittur/gargoyle-account-profile) | account-profile service | [:8001](http://localhost:8001) |
| [🦒 griffin-tweet](https://github.com/VL037-twittur/griffin-tweet) | tweet service | [:8002](http://localhost:8002) |
| [🦊 harpy-communication](https://github.com/VL037-twittur/harpy-communication) | communication service | [:8003](http://localhost:8003) |
| [🦝 kraken-information](https://github.com/VL037-twittur/kraken-information) | information service | [:8004](http://localhost:8004)

---

#### 🎭 System Design

<img src="https://github.com/VL037-twittur/.github/assets/68309124/9ab9ab40-5e36-45c1-84ec-f1d41364e639" alt="Twittur System Design" width="600">

---

#### 👵 How to run?

| Tool              | Detail |
|-------------------|--------|
| Java  (JAVA_HOME) | [17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) |
| Spring Boot       | 3.0.4 |
| Databases         | [PostgreSQL](https://www.postgresql.org/download), [MongoDB](https://www.mongodb.com/try/download/community), [Redis](https://github.com/ServiceStack/redis-windows/tree/master/downloads) |
| Message Broker    | [Apache Kafka](https://kafka.apache.org/downloads) |
| Email Service     | Gmail SMTP |
| IDE               | [Intellij IDEA Community Edition](https://www.jetbrains.com/idea/download) |
| Build tool        | [Maven 3.6.3](https://archive.apache.org/dist/maven/maven-3/3.6.3) |

- `git clone` all services
- Run `databases` & `message broker` locally
- Create Database named `twittur`
- run `mvn clean install` on [abomination-base](https://github.com/VL037-twittur/abomination-base)
- run `mvn spring-boot:run` on [twittur-db-migration](https://github.com/VL037-twittur/twittur-db-migration)
- run `mvn spring-boot:run` on [basilisk-registry](https://github.com/VL037-twittur/basilisk-registry)
- run all other services on your `IDE`
- open [localhost:8761](http://localhost:8761) and make sure all services are up <img alt="Eureka Registry" src="https://github.com/VL037-twittur/.github/assets/68309124/8db0840f-083f-4a85-9f3d-d5b5b0e2d5a2" width="600">
- you can hit the apis from the [gateway port](http://localhost:8080) but is still on-going, and api spec not ready. Please refer to every service port.

---

🍿 Care to join? [DM me!](https://www.linkedin.com/in/vinc)

