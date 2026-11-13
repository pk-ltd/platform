# 1. Repository structure

Date: 2026-11-13
Status: Accepted

## Context
Pipelines, permissions and credentials are scoped per repository. Infrastructure,
GitOps and application code have different owners, change rates and blast radius.
The structure must grow by adding, not by reorganising.

## Decision
Use a GitHub organization (pk-ltd) with repositories split by lifecycle:
platform, ci-templates, demo-app, packer-images, terraform-modules,
ansible-collection-homelab, infra-live, platform-gitops, apps-gitops.
Modules, roles and images are versioned; infra-live pins versions.
All repositories are public except infra-live; no secrets are stored in Git.

## Consequences
- Each repository has one pipeline with least-privilege permissions.
- Only infra-live holds infrastructure credentials.
- Cross-repo changes need several PRs.
- Free-plan rulesets apply to public repositories only.
