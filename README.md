## How to run?

### Build all modules:

`spring-boot-microservices-series> ./mvnw clean package -DskipTests=true`

### Start infrastructure modules in docker:

**The simplest way to run all the services in Docker:**

`spring-boot-microservices-series> ./run.sh start_all`

**To start only infrastructure services (mysqldb, rabbitmq, config-server, service-registry, hystrix-dashboard) in docker:**

`spring-boot-microservices-series> ./run.sh start_infra`

**Start each microservice either in local or in docker:**

**Local:** `spring-boot-microservices-series/catalog-service> ./mvnw spring-boot:run`

**Docker:** `spring-boot-microservices-series> ./run.sh start <service>`

Ex: `spring-boot-microservices-series> ./run.sh start catalog-service`