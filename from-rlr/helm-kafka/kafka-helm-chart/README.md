# Kafka (Single-broker KRaft) Helm Chart

## Install
```bash
helm install kafka /path/to/kafka-helm-chart -n kafka --create-namespace
```

## Customize
Edit `values.yaml` to set image, ports, and all Kafka env vars under `env:`.
For external access, set:
```yaml
service:
  public:
    enabled: true
    type: LoadBalancer
```
and update `KAFKA_ADVERTISED_LISTENERS` accordingly.
