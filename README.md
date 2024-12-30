# [Intro to databases](https://btholt.github.io/complete-intro-to-databases/)

## 4 major types

### Document-Based (NoSQL)

* Advantage: Your data is totally unstructured. Can get started fast. Most are Javascript based queries so it is easy to integrate.
* Disadvantage: It can even be a bit of a problem when you misspell field names since the database will just happily accept the misspelled field name
* When you say NoSQL, you're basically saying it's just not a relational database
* Examples: MongoDB / Cassandra / Couchbase / ReThinkDB

#### Indexes

* Separate data structure that a database maintains so that it can find things quickly
* The tradeoff here is that indexes can cause inserts, updates, and deletes to be a bit slower because they also have to update indexes as well as they just take up more room on disk. But in exchange you get very fast queries as well as some other neat properties like enforcing unique keys.

#### Cloud solutions

* MongoDB Atlas / Microsoft Azure Cosmos DB / Amazon Web Services DocumentDB

### Relational (RDBMS / SQL)

* Examples: MySQL

### Graph

* Examples: Neo4j

### Key-Value store

* Examples: Redis

## Other types

### Search engines

* Examples: Solr / sphinx
* They are often paired with databases to make search possible

### Wide column

* Examples: Apache Cassandra / Google Bigtable
* Two dimensional key-value store
* Capable of massive scale and is very resilient

### Message brokers

* Examples: Apache Kafka / RabbitMQ / Celery
* They allow apps and services to publish events/messages on a system and allow the message broker to publish/inform subscribers to those events that something happened.

### Multi model

* Examples: Azure Cosmos DB / ArangoDB
* Databases that can operate in multiple different ways listed above