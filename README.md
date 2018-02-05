# 2018-feb-kafkatcp
TCP server implementing kafka protocol to include avro-schema-validation of producer messages

## TCP Binary
Kafka Protocol is a description of the byte sequence expected over TPC
https://cwiki.apache.org/confluence/display/KAFKA/A+Guide+To+The+Kafka+Protocol#AGuideToTheKafkaProtocol-ProduceRequest
A implementation in Golang https://github.com/travisjeffery/jocko/tree/master/protocol

Can we implement the HTTP binary protocol in our own TCP server, like Kafka does?
Does this mean we can we avoid TLS handsake, if so: what are the security implications? What should be mitigated?

Can we include checking of schemas before writing it to Kafka?

https://github.com/dpkp/kafka-python/blob/master/kafka/client.py#L609
https://github.com/dpkp/kafka-python/blob/master/kafka/producer/base.py#L432
