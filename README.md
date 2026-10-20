# homelab-ansible

Ansible roles that turn plain Debian/Ubuntu VMs into a kubeadm-based Kubernetes cluster.
Part of my personal DevOps homelab.

## Status

Work in progress: manual install notes first, automation next.

## Planned structure

- `inventories/lab/` – lab hosts
- `roles/` – common, containerd, kubernetes_node, control_plane, worker, cni_calico
- `playbooks/site.yml` – builds the whole cluster
- `docs/` – manual install notes, ADRs, runbooks
