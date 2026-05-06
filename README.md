# NovaPay Zero-Downtime CI/CD Pipeline

## Overview

This project designs a production-grade CI/CD pipeline for a digital banking system (NovaPay). The goal is to achieve:

* Zero-downtime deployments
* Automated compliance enforcement (RBI + PCI-DSS)
* Secure and fast delivery (<2 hours)

## Architecture

The pipeline consists of 8 stages:

1. Source Control
2. Build & Test
3. SAST
4. Dependency Scan
5. Integration Testing
6. DAST
7. Compliance Gates
8. Deployment

## Deployment Strategy

* Blue-Green deployment for instant switching
* Canary deployment for gradual rollout

## Key Features

* Automated rollback
* Expand-contract DB migration
* 4-environment promotion model
* Observability with DORA metrics

## Structure

* docs/ → all deliverables
* pipeline/ → CI/CD configs
* runbooks/ → operational guides
* dashboards/ → monitoring
* evidence/ → submission files
