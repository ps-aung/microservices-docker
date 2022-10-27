# SpringBoot Microservices with docker

## Installing Tools

- Used 17.0.4.1 of Java
- Used 2022-09 of "Eclipse IDE for Enterprise Java and Web Developers" or "Intelliji IDEA Community Edition 2022.2.3"
- Used Spring Boot 2.7.5 works only with Java 17+

## Images

- https://hub.docker.com/u/pyaesoneag
- Currency Exchange Service 
	- pyaesoneag/mmv2-currency-exchange-service:0.0.1-SNAPSHOT
- Currency Conversion Service
	- pyaesoneag/mmv2-currency-conversion-service:0.0.1-SNAPSHOT
- Eureka
	- pyaesoneag/mmv2-naming-server:0.0.1-SNAPSHOT
- API GATEWAY
	- pyaesoneag/mmv2-api-gateway:0.0.1-SNAPSHOT

## URLS

#### Currency Exchange Service
- http://localhost:8000/currency-exchange/from/USD/to/MMK

#### Currency Conversion Service
- http://localhost:8100/currency-conversion/from/USD/to/MMK/quantity/10

#### Eureka
- http://localhost:8761/

#### Zipkin
- http://localhost:9411/

#### API GATEWAY
- http://localhost:8765/currency-exchange/from/USD/to/MMK
- http://localhost:8765/currency-conversion/from/USD/to/MMK/quantity/10
- http://localhost:8765/currency-conversion-new/from/USD/to/MMK/quantity/10

#### Commands
```
docker run -p {host_port}:{docker_port} -d {image_name}:{tag}
docker-compose --version
docker-compose up
```
