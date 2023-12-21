# Docker

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
docker-compose --version
docker-compose up
watch -n 0.1 curl http://localhost:8000/sample-api
```
