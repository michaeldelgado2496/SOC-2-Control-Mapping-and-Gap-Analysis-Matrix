# TacoTrax Encryption Standards
**Effective Date:** September 17, 2026  
**Scope:** Customer delivery data, database records, and transit transmissions.

## 1. Encryption in Transit
- All external and internal communications must be encrypted using Transport Layer Security (TLS) version 1.3.
- Weak or deprecated ciphers are automatically blocked by cloud load balancers.

## 2. Encryption at Rest
- All databases and storage buckets housing customer PII and proprietary recipes must be encrypted using AES-256.
- Encryption keys are managed via cloud-native Key Management Services (KMS) with automated annual rotation.
