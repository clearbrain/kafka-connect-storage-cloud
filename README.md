# Kafka Connect Suite of Cloud Storage Connectors

## ClearBrain Notes:
This repo is forked from the confluent project for the purpose of updating the TopicPartitionWriter (as of 2017/9/7) to allow for the S3 Sink to flush files to S3 at a schedule cadence regardless of whether the flush size hits the configured limit (15000 records)

*kafka-connect-storage-cloud* is a suite of [Kafka Connectors](http://kafka.apache.org/documentation.html#connect)
designed to be used to copy data between Kafka and public cloud stores, such as Amazon S3. The currently available connectors are listed below:

## Kafka Connect Sink Connector for Amazon Simple Storage Service (S3)

Documentation for this connector can be found [here](http://docs.confluent.io/current/connect/connect-storage-cloud/kafka-connect-s3/docs/index.html).

# Development

To build a development version you'll need a recent version of Kafka. You can build
*kafka-connect-storage-cloud* with Maven using the standard lifecycle phases.


# Contribute

- Source Code: https://github.com/confluentinc/kafka-connect-storage-cloud
- Issue Tracker: https://github.com/confluentinc/kafka-connect-storage-cloud/issues


# License

The project is licensed under the Apache 2 license.
