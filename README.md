# kafka_PoC
**Running Kafka**

1. Run cmd
2. goto kafka/bin/windows
3. Run zookeeper by running commnd "zookeeper-server-start.bat ../../config/zookeeper.properties"
4. After zookeper has started succesfully RUn kafka by running command "kafka-server-start.bat ../../config/server.properties"

**Creating a topic**

1. Run cmd
2. goto kafka/bin/windows
3. Run "kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test"
4. This will create a topic 'test' on kafka.

**Run Producer**

1. Open cmd
2. Goto kafka_Poc folder
3. Run "npm run start:producer"

**Run Consumer**

1. Open cmd
2. Goto kafka_Poc folder
3. Run "npm run start:consumer"



Code exmaple followed from : https://github.com/kriscfoster/node-kafka-producer-consumer
