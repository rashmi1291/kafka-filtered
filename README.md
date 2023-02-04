## Kafka filtered listener demo project

The project exposes a simple rest endpoint to publish the message to a kafka topic using spring kafka's KafkaTemplate.

The project has a filtered listener which only consumes the messages that meets the filtered criteria based on the filter criteria (eventType)

### Versions:
Spring boot: 3.0.2
Apache Kafka: 3.3.2


### To start:
Run the KafkaFilteredApplication as main spring boot application.


### Request endpoint
### POST:
http://localhost:8080/publish

### BODY:
#### Request 1
{
"eventType": "NEWM",
"message": "NEW message consumed."
}

#### Request 2
{
"eventType": "CANC",
"message": "Cancel message skipped."
}



    

