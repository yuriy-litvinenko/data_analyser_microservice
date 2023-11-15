# data_analyser_microservice

## Описание проекта
Учебный проект, представляющий собой сервис для принятия и обработки тестовых данных из Apache Kafka, 
отправленных посредством микросервиса data-generator-microservice.

Общие возможности сервиса:
- Прием и обработка сообщений из Apache Kafka

## Стек технологий
- **Java 17.0.4.1**
- **Spring Boot 3.1.5**
- **Lombok 1.18.28**
- **MapStruct 1.5.5**
- **Spring Kafka 3.0.12**
- **Reactor Kafka 1.3.21**
- **Jcabi XML 0.29.0**
- **Gson 2.10.1**

## Использованное окружение при тестировании сервиса
- **Java 17.0.4.1**
- **Maven 3.6.2**
- **Kafka 2.13-3.6.0**

## Взаимодействие с приложением
1. **Запуск ZooKeeper**  
   .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
2. **Запуск Kafka**  
   .\bin\windows\kafka-server-start.bat .\config\server.properties
3. **Мониторинг поступивших в Kafka сообщений с заданным топиком**  
   .\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic data-temperature --from-beginning
