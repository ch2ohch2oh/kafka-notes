# Hitchhikers's Guide on Kafka

20 min talk by Lucia Cerchie from 
[Kafka Summit London 2023](https://www.confluent.io/events/kafka-summit-london-2023/a-hitchhikers-guide-to-apache-kafka-r/).
No hands-on.

## What
Apache kafka is an event streaming middleware.

## Features

- Each event is stored in a log.
- Events are durable and cannot be mutated.
- Events can be deleted.
- Events are partitioned. The partition key is assigned by the producer.
- The producer will compress the data.

## Configs

THe producer configures
- `batch.size`
- `linger.ms`

The consumers can
- read from many topics.
- be organized in groups.

The consumer needs to keep an eye on 
- `group.id`
- `request.timeout.ms`
- `retries`

## Buzzwords

- Scalability
- Fault tolerance
- Real-time processing

