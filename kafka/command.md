
```shell
# 创建topic
docker exec kafka kafka-topics.sh --create --zookeeper zookeeper:2181 --replication-factor 1 --partitions 1 --topic <主题名>

# 删除topic
docker exec kafka kafka-topics.sh --delete --zookeeper zookeeper:2181 --topic <主题名>

# 查看topics
docker exec kafka kafka-topics.sh --list --zookeeper zookeeper:2181

# 创建消息生产者
docker exec -it kafka kafka-console-producer.sh --broker-list kafka:9092 --topic <主题名>

# 消费者
docker exec -it kafka kafka-console-consumer.sh --bootstrap-server kafka:9092 --topic <主题名> --from-beginning
```
