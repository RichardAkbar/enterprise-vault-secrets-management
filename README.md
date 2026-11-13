# Enterprise Vault Secrets Management

An enterprise-oriented secrets management project using HashiCorp Vault to centralize, secure, and manage application credentials and sensitive infrastructure data.

## Project Overview

This project demonstrates how HashiCorp Vault can be used to manage secrets securely across infrastructure and application environments.

The implementation focuses on centralized secrets storage, identity-based authentication, fine-grained access control, dynamic database credentials, and security auditing.

## Objectives

- Deploy and inspect HashiCorp Vault.
- Implement centralized secrets management.
- Configure KV Secrets Engine v2.
- Implement authentication and authorization.
- Configure AppRole authentication.
- Generate dynamic MySQL database credentials.
- Integrate Vault with Kubernetes workloads.
- Implement secret lifecycle management.
- Enable audit logging and perform security testing.

## Technology Stack

| Technology | Purpose |
|---|---|
| HashiCorp Vault | Secrets management |
| MySQL | Database integration |
| Linux / Ubuntu | Infrastructure environment |
| Kubernetes | Container orchestration integration |
| Git & GitHub | Version control and documentation |

## Architecture

The platform uses HashiCorp Vault as a centralized security layer.

Applications authenticate to Vault using approved authentication methods and retrieve only the secrets permitted by their assigned policies.

Dynamic database credentials are generated through Vault's Database Secrets Engine.

## Project Checkpoints

| Checkpoint | Description |
|---|---|
| CP01 | Environment Discovery & Validation |
| CP02 | Vault Architecture & Configuration |
| CP03 | Authentication & Root Security |
| CP04 | KV Secrets Engine v2 |
| CP05 | AppRole & Access Policies |
| CP06 | Dynamic MySQL Credentials |
| CP07 | Kubernetes Integration |
| CP08 | Secret Lifecycle Management |
| CP09 | Audit Logging & Security Testing |
| CP10 | Documentation & Portfolio |

## Repository Structure

```text
.
├── architecture/
├── configs/
│   ├── vault/
│   ├── policies/
│   └── kubernetes/
├── database/
│   └── mysql/
├── docs/
├── evidence/
├── scripts/
├── .gitignore
└── README.md
```

## Security Considerations

- Never commit Vault root tokens or unseal keys.
- Never store plaintext credentials in source control.
- Use least-privilege access policies.
- Prefer TLS for production Vault deployments.
- Use short-lived dynamic credentials where appropriate.
- Protect audit logs and sensitive configuration files.

## Implementation Status

Project initialization and environment discovery are in progress.

Detailed implementation steps, validation results, and evidence will be documented throughout the project checkpoints.

## Disclaimer

This repository is intended for educational and portfolio purposes. The playground configuration is not a production-ready deployment.

Production environments require additional hardening, secure TLS configuration, appropriate high availability, backup and recovery procedures, and operational security controls.
