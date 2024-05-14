
# Using Confluent
FROM confluentinc/cp-kafka-connect:latest

# RUN confluent-hub install confluentinc/kafka-connect-hdfs3:1.1.30 --no-prompt --verbose [subscribe]
# RUN confluent-hub install confluentinc/kafka-connect-hdfs3-source:2.5.17 --no-prompt --verbose
# RUN confluent-hub install debezium/debezium-connector-postgresql:2.5.3 --no-prompt --verbose
# RUN confluent-hub install debezium/debezium-connector-sqlserver:2.4.2 --no-prompt --verbose
# RUN confluent-hub install debezium/debezium-connector-mongodb:2.4.2 --no-prompt --verbose
# RUN confluent-hub install debezium/debezium-connector-mysql:2.4.2 --no-prompt --verbose

COPY ./debezium-connector-oracle/* /usr/share/confluent-hub-components/debezium-connector-oracle/
COPY ./hdfs-sink-connector /usr/share/confluent-hub-components/hdfs-sink-connector
COPY ./oracle_driver/ojdbc8.jar /usr/share/java/kafka/ojdbc8.jar