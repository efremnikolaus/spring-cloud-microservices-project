# Docker

## Images

- https://hub.docker.com/repositories/nikolai7
- nikolai7/api-gateway:latest
- nikolai7/currency-conversion-service:latest
- nikolai7/currency-exchange-service:latest
- nikolai7/naming-server:latest

- openzipkin/zipkin:latest

## URLS

#### Currency Exchange Service
- http://localhost:8000/currency-exchange/from/USD/to/UAH

#### Currency Conversion Service
- http://localhost:8100/currency-conversion/from/USD/to/UAH/quantity/10
- http://localhost:8100/currency-conversion-feign/from/USD/to/UAH/quantity/10

#### Eureka
- http://localhost:8761/

#### Zipkin
- http://localhost:9411/

#### API GATEWAY
- http://localhost:8765/currency-exchange/from/USD/to/UAH
- http://localhost:8765/currency-conversion/from/USD/to/UAH/quantity/10
- http://localhost:8765/currency-conversion-feign/from/USD/to/UAH/quantity/10
- http://localhost:8765/currency-conversion-new/from/USD/to/UAH/quantity/10

#### Commands
```
mvn clean install -DskipTests
docker run -p 9411:9411 openzipkin/zipkin:latest
docker-compose up
docker-compose down
watch -n 0.1 curl http://localhost:8000/sample-api
```
