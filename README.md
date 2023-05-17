# Kafka Connect Docker Image

Docker file for building docker image for [Kafka Connect](https://kafka.apache.org/documentation/#connect) bundled with a couple of free connectors from [Confluent Hub](https://www.confluent.io/hub/).

The following connectors from [Confluent Hub](https://www.confluent.io/hub/) are bundled into the docker image:

- JDBC Connect (Source and Sink)
- Kafka Connect HDFS
- Kafka Connect Elasticsearch
- Amazon S3 Sink Connector
- Kafka Connect Avro Converter

Available connector classes:

```json
[
    {
        "class": "io.confluent.connect.elasticsearch.ElasticsearchSinkConnector",
        "type": "sink",
        "version": "11.0.0"
    },
    {
        "class": "io.confluent.connect.hdfs.HdfsSinkConnector",
        "type": "sink",
        "version": "10.0.0"
    },
    {
        "class": "io.confluent.connect.hdfs.tools.SchemaSourceConnector",
        "type": "source",
        "version": "6.0.1-ccs"
    },
    {
        "class": "io.confluent.connect.jdbc.JdbcSinkConnector",
        "type": "sink",
        "version": "10.0.1"
    },
    {
        "class": "io.confluent.connect.jdbc.JdbcSourceConnector",
        "type": "source",
        "version": "10.0.1"
    },
    {
        "class": "io.confluent.connect.s3.S3SinkConnector",
        "type": "sink",
        "version": "5.5.3"
    },
    {
        "class": "io.confluent.connect.storage.tools.SchemaSourceConnector",
        "type": "source",
        "version": "6.0.1-ccs"
    },
    {
        "class": "org.apache.kafka.connect.file.FileStreamSinkConnector",
        "type": "sink",
        "version": "6.0.1-ccs"
    },
    {
        "class": "org.apache.kafka.connect.file.FileStreamSourceConnector",
        "type": "source",
        "version": "6.0.1-ccs"
    },
    {
        "class": "org.apache.kafka.connect.mirror.MirrorCheckpointConnector",
        "type": "source",
        "version": "1"
    },
    {
        "class": "org.apache.kafka.connect.mirror.MirrorHeartbeatConnector",
        "type": "source",
        "version": "1"
    },
    {
        "class": "org.apache.kafka.connect.mirror.MirrorSourceConnector",
        "type": "source",
        "version": "1"
    }
]
```