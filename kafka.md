# kafka

Brokers, Producers, Consumers, and Zookeeper - Scaler Topics. In Kafka, a producer sends messages to a topic, which is divided into partitions for parallel processing.
These partitions are stored by brokers within a Kafka cluster, which are coordinated by ZooKeeper. Consumers subscribe to topics and read messages from partitions, tracking their progress using an offset.

* producer
* topic
* partition
* consumer/group
* broker
* zookeeper
* offset
* kafka cluster

## Producers
Send data (messages) to Kafka topics. Can optimize message delivery by balancing, serializing, and compressing messages across partitions.

## Topics
Logical categories for storing messages. Messages within a topic are organized into partitions.

## Partitions
Subdivisions of a topic that hold messages in an ordered, immutable sequence. Enable parallel processing by allowing multiple consumers to read different partitions simultaneously.

## Brokers
Kafka servers that store data, handle read/write requests, and manage partitions. They form a Kafka cluster and distribute the data load across the cluster.

## Kafka Cluster
A collection of one or more brokers working together to provide high availability, scalability, and fault tolerance.

## ZooKeeper (or KRaft)
Used for cluster coordination and managing metadata. Tracks the status of brokers, performs leader election for partitions, and notifies producers and consumers of cluster changes.

## Consumers
Subscribe to topics to read messages. Pull messages from partitions rather than having them pushed by Kafka.

## Consumer Group
A group of consumers that share the responsibility of consuming messages from a topic. Each partition in a topic is consumed by only one consumer within a given group, ensuring each message is processed only once by the group.

## Offset
A unique, sequential identifier for each message within a partition. Consumers maintain a record of the last consumed offset for each partition, allowing them to resume reading from where they left off after a crash or restart.
