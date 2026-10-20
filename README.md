# homelab

Personal DevOps homelab built entirely as code:
Packer → Terraform → Ansible → Kubernetes (kubeadm) → Argo CD.

Application source code lives in a separate repository: [demo-app](https://github.com/peterkroushovsky/demo-app).

## Layout

| Path | Purpose |
| --- | --- |
| `infrastructure/packer` | Golden VM images |
| `infrastructure/terraform` | VMs and networks (local, Oracle Cloud, AWS) |
| `infrastructure/ansible` | Node configuration and cluster install |
| `kubernetes/bootstrap` | Argo CD installation |
| `kubernetes/platform` | Cluster services (networking, storage, monitoring) |
| `kubernetes/apps` | Application deployments managed by Argo CD |
| `docs/` | ADRs and runbooks |

## Status

Work in progress.
