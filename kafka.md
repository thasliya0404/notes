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

## Notes
![2288c087-0e06-496f-a460-fc66f69cda8a](https://github.com/user-attachments/assets/c110f18e-98af-4da1-a8e6-277a596c6102)

![04b9f8cf-61cb-4919-9981-c0c4b97247f4](https://github.com/user-attachments/assets/9f386452-5ca6-4b65-b4b2-1b448e1f83f4)

![8ed7ea79-2cc5-46b4-a1f2-8ea2f414e491](https://github.com/user-attachments/assets/15ab7aab-f1a9-480a-932a-cff6866a17dd)

![362127fd-9e5b-4c1d-b396-a0d04d2866eb](https://github.com/user-attachments/assets/1c70ab7e-461e-4d37-9d19-086582434877)

![2761d26c-dfc5-41a8-8ace-24ba0feec1f8](https://github.com/user-attachments/assets/1f019c49-f026-4027-8005-3cc355fabc34)

![2cc5c085-8726-4a91-bfc2-95adeefc6273](https://github.com/user-attachments/assets/2310cbbc-12ca-48db-85dc-df1f064fb76e)

![c9d0fcda-d647-44aa-9c7b-42f3900c5340](https://github.com/user-attachments/assets/df32559f-08ed-4148-82d1-c00b2b11fa60)

![442fe406-16d7-41c6-a7d3-b4f3ccdfd5d4](https://github.com/user-attachments/assets/b223aac0-7f3f-4796-977b-4d108b55a23e)

![Capture 1](https://github.com/user-attachments/assets/da4d0d79-cd32-42c1-81a7-80b8cc5ecc2d)

<img width="2560" height="1440" alt="Screenshot (110)" src="https://github.com/user-attachments/assets/83dbc6bb-bacb-4fd5-bc19-00ad68c007fb" />

<img width="2560" height="1440" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/f0da1c62-6c6c-4680-9871-5c5f1db5f72a" />

<img width="2560" height="1440" alt="Screenshot (112)" src="https://github.com/user-attachments/assets/0249c8f1-cd9f-4855-9b25-c7df4bf8a819" />

<img width="2560" height="1440" alt="Screenshot (113)" src="https://github.com/user-attachments/assets/d10070db-768a-4399-adfb-c845b85baeb7" />

<img width="2560" height="1440" alt="Screenshot (114)" src="https://github.com/user-attachments/assets/4a8dcc0f-f22d-4c47-a5cf-a8f983d2b7e3" />

<img width="2560" height="1440" alt="Screenshot (115)" src="https://github.com/user-attachments/assets/45bc38e5-399b-49a3-896c-2317f1637ec3" />

<img width="2560" height="1440" alt="Screenshot (116)" src="https://github.com/user-attachments/assets/ba198939-a155-4997-ac58-a99960d42e74" />

<img width="2560" height="1440" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/42a52ddd-8202-48b6-a8a3-117748b389dd" />

<img width="2560" height="1440" alt="Screenshot (118)" src="https://github.com/user-attachments/assets/ec3f4d84-6aef-424e-bcde-41dc628fd017" />

<img width="2560" height="1440" alt="Screenshot (119)" src="https://github.com/user-attachments/assets/31bc071c-ece8-4764-920a-1279ce295444" />

<img width="1903" height="1173" alt="Screenshot (120)" src="https://github.com/user-attachments/assets/ee5097ea-0a28-4ede-95b4-7b2ac6ec6570" />

<img width="2560" height="1440" alt="Screenshot (121)" src="https://github.com/user-attachments/assets/495a3931-ae03-4a86-bf9f-c46361512084" />

<img width="2560" height="1440" alt="Screenshot (122)" src="https://github.com/user-attachments/assets/24d16938-69a1-430c-ad01-43a90e99bf2b" />










