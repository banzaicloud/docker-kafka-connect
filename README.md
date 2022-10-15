# Kafka Connect Docker Image

Docker file for building docker image for [Kafka Connect](https://kafka.apache.org/documentation/#connect) bundled with a couple of free connectors from [Confluent Hub](https://www.confluent.io/hub/).

The following connectors from [Confluent Hub](https://www.confluent.io/hub/) are bundled into the docker image:

- JDBC Connect (Source and Sink)
- Kafka Connect HDFS
- Kafka Connect Elasticsearch
- Amazon S3 Sink Connector
- Kafka Connect Avro Converter
- Kafka Connect Spooldir (https://docs.confluent.io/kafka-connectors/spooldir/current/overview.html)

Available connector classes in the latest build are:

- io.confluent.connect.elasticsearch.ElasticsearchSinkConnector
- io.confluent.connect.hdfs.HdfsSinkConnector
- io.confluent.connect.jdbc.JdbcSinkConnector
- io.confluent.connect.s3.S3SinkConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirAvroSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirBinaryFileSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirCsvSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirJsonSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirLineDelimitedSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.SpoolDirSchemaLessJsonSourceConnector
- com.github.jcustenborder.kafka.connect.spooldir.elf.SpoolDirELFSourceConnector
- io.confluent.connect.hdfs.tools.SchemaSourceConnector
- io.confluent.connect.jdbc.JdbcSourceConnector
- io.confluent.connect.storage.tools.SchemaSourceConnector
- org.apache.kafka.connect.mirror.MirrorCheckpointConnector
- org.apache.kafka.connect.mirror.MirrorHeartbeatConnector
- org.apache.kafka.connect.mirror.MirrorSourceConnector
