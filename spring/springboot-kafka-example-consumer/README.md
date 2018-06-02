# Spring Boot Kafka example consumer
Example of Spring Boot Kafka replying consumer. 

## How to use
**1. Clone the application**

```bash
git clone https://gitlab.com/harvan/example.git
```

**2. Download & install kafka**

```bash
https://kafka.apache.org/downloads
https://kafka.apache.org/quickstart
```

**3. Build the application**

```bash
mvn clean install
```

**4. Go to kafka directory**

```bash
localDrive>cd D:\app\kafka_2.12-1.1.0
```

**5. Run the kafka server**

```bash
D:\app\kafka_2.12-1.1.0>.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
D:\app\kafka_2.12-1.1.0>.\bin\windows\kafka-server-start.bat .\config\server.properties
```

**6. Run the spring boot application**

```bash
java -jar -Dserver.port=8082 target/springboot-kafka-example-consumer-0.0.1-SNAPSHOT-exec.jar
```

**7. Access the application via kafka**

```
Topic   = request-topic
Payload =
{
	"firstNumber": 1,
	"secondNumber":2
}
```