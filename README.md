# K8S SigNoz Infra Monitoring

## 🛠 Setup Instructions

### Prerequisites

- Kubernetes cluster (tested on vSphere)
- Helm installed
- Ansible installed
- SigNoz running on Docker (collector reachable via host IP)

### 🔼 To Deploy Agent

```bash
ansible-playbook ansible/up.yaml
```

### 🔽 To Uninstall Agent

```bash
ansible-playbook ansible/down.yaml
```

## 📦 What’s Included

- `up.yaml` and `down.yaml`: Ansible playbooks
- `values.yaml`: Helm chart override for OTEL collector IP/port
- `screenshots/`: Add proof of SigNoz monitoring working

## ✅ Tasks Done

- [x] SigNoz collector setup on TrueNAS
- [x] Installed k8s-infra agent via Ansible
- [x] Used Helm values to override collector IP
- [x] Deployed `rolldice` app and verified telemetry
- [x] Tested on vSphere

## 📸 Screenshots

- SigNoz hosts
- Metrics showing up
- Rolldice telemetry
- vSphere nodes visible
