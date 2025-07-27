# SigNoz K8s Infra Setup via Ansible

This repo sets up the Signoz K8s Infra agent to forward telemetry to a SigNoz collector running in Docker (e.g. on TrueNAS).

## Usage

```bash
# Install
ansible-playbook ansible/up.yaml -i ansible/inventory.yaml

# Uninstall
ansible-playbook ansible/down.yaml -i ansible/inventory.yaml
```

## Customization

Edit `helm/values.yaml` to point to your OTEL collector.

## Test App

Deploy `manifests/rolldice-deployment.yaml` to test telemetry capture.
