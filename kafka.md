# Important Commands: Kafka
---

Start Zookeeper Server
```
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```

Start Kafka Server
```
.\bin\windows\kafka-server-start.bat .\config\server.properties
```

List of topics in Kafka
```
.\bin\windows\kafka-topics.bat --list --zookeeper localhost:2181
```

Create topic
```
kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic <topic-name>
kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test
```

Producer Topic
```
kafka-console-producer.bat --broker-list localhost:9092 --topic <topic-name>
kafka-console-producer.bat --broker-list localhost:9092 --topic test
```

Consumer Topic
```
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic <topic-name>
kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic test
```

# References
[Kafka Tutorials](https://dzone.com/articles/running-apache-kafka-on-windows-os)
