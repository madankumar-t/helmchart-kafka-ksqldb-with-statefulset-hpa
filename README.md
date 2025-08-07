# Confluent LocalDev Helm Chart

This Helm chart deploys the following components into an EKS cluster using Confluent's localdev container images:

- Kafka Broker
- ksqlDB Server
- Schema Registry

## Deployment

```bash
helm install confluent-localdev ./confluent-localdev
```

## Configuration

All configuration options are set in `values.yaml`.
