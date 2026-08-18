# Averixa Group — Deployment Standards

## Purpose

This document defines the general deployment standards for Averixa Group applications and services.

The objective is to establish a secure, repeatable, observable, and scalable deployment process while keeping development, staging, and production environments properly separated.

---

## Deployment Principles

Averixa Group deployments should follow these principles:

1. Production code must originate from version control.
2. Production credentials must never be committed to Git.
3. Deployments should be reproducible.
4. Automated validation should occur before production deployment.
5. Production and development environments must remain separated.
6. Deployments should support rollback when practical.
7. Infrastructure changes should be documented.
8. Applications should expose appropriate health checks.
9. Production systems should be monitored.
10. Deployment permissions should follow the principle of least privilege.

---

## Environments

Applications should normally support three environments:

```text
development
staging
production
