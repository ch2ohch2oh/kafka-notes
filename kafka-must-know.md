# Kafka Must Know

My condensed note based on the four-part blog posts:
1. [Streams and Tables in Apache Kafka: A Primer](https://www.confluent.io/blog/kafka-streams-tables-part-1-event-streaming/)


## What

Kafka is an event streaming platform.


## Key concepts

### Event

An **event** records the fact that “something happened” in the world. Conceptually, an event has a key, value, and timestamp. 

### Stream

An event stream records the history of what has happened in the 
world as **a sequence of events**.

### Event vs table

Compared to an event stream, a table represents the state of the world 
at a particular point in time, typically “now.”

In terms of mutability

- A stream provides **immutable** data. 
- A table provides **mutable** data. 

### Stream-table duality

- We can turn a stream into a table by aggregating the stream 
of updates.
- We can turn a table into a stream by capturing the changes made 
to the table—inserts, updates, and deletes—into a “change stream.”

The key observation is: a table is fully defined by its underlying change stream.

