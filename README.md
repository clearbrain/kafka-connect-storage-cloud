# Kafka Connect Suite of Cloud Storage Connectors

## ClearBrain Notes:
This repo is forked from the confluent project for the purpose of updating the TopicPartitionWriter (as of 2017/9/7) to allow for the S3 Sink to flush files to S3 at a schedule cadence regardless of whether the flush size hits the configured limit (15000 records)

Deployment Steps:
1. Ensure that you have maven installed on your computer
2. Run `mvn package`.  This will build the jars
3. Copy the file `kafka-connect-s3/target/kafka-connect-s3-4.0.0-SNAPSHOT-package/share/java/kafka-connect-s3/kafka-connect-s3-4.0.0-SNAPSHOT.jar` to the kafka cluster under `/home/ec2-user/confluent-3.3.0/share/java/kafka-connect-s3`.  You can use scp or any ftp tool (make sure that it doesn't get copied as 0 bytes).  Make sure to move/remove any existing jar under the target directory that has a name prefixed with `kafka-connect-s3` (we are trying to overwrite the file).



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
