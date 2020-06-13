# Kafka and ElasticSearch


This application will consume tweets from a Kafka broker and send them to ElasticSearch.

### Useful commands

### Start Zookeeper
```
zookeeper-server-start.bat config\zookeeper.properties
```

### Start Kafka
```
kafka-server-start.bat config\server.properties
```

### Create 'twitter_tweets' Topic
```
kafka-topics --bootstrap-server localhost:9092 --create --topic twitter-tweets --partitions 6 --replication-factor 1
```

### Kafka Console Consumer
```
kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic twitter_tweets
```
