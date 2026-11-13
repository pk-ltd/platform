# platform

Entry point to the pk-ltd homelab: roadmap, architecture decisions, runbooks and the shared backlog.

## Repositories

| Repository | Purpose |
| --- | --- |
| [demo-app](https://github.com/pk-ltd/demo-app) | Sample Go service: build, scan, sign, publish image |
| [ci-templates](https://github.com/pk-ltd/ci-templates) | Reusable GitHub Actions workflows |
| [apps-gitops](https://github.com/pk-ltd/apps-gitops) | Application deployment config (Argo CD) |
| [platform-gitops](https://github.com/pk-ltd/platform-gitops) | Cluster platform components (Argo CD) |
| infra-live (private) | Live environments: Terraform and Ansible |
| terraform-modules *(planned)* | Versioned Terraform modules |
| ansible-collection-homelab *(planned)* | Versioned Ansible roles |
| packer-images *(planned)* | Golden VM images |

## Layout

| Path | Purpose |
| --- | --- |
| `docs/adr/` | Architecture Decision Records |
| `docs/runbooks/` | Operational runbooks |
| `docs/notes/` | Learning notes |
