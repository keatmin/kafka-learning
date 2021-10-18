## Setup 1. Run `docker compose -d up` 
2. Run
```bash
docker compose exec broker \
  kafka-topics --create \
    --topic purchases \
    --bootstrap-server localhost:9092 \
    --replication-factor 1 \
    --partitions 1
```
3. Produce and consume

### TODO
- figure out how to test
- how to work with schema registry with avro
