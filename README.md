# kafka-zookeeper

1)This command is used to start the Zookeeper service 
`` .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties ``

2)This command is used to start Kafka service 
``.\bin\windows\kafka-server-start.bat .\config\server.properties ``

3)This command is used to craete topic in kafka 
`` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic Gampa-testing-topic ``

4)This command is used to list the created topics
`` .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list ``

5)This command is used to compile and build jar file.
```mvn clean compile assembly:single```

6)This command is used to run kafka producer
`` java -cp target/kafka-zookeeper-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatakafka.CustomProducer test ``

7)This command is used to run consumer 
`` java -cp target/kafka-zookeeper-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatakafka.CustomConsumer test group1 ``
