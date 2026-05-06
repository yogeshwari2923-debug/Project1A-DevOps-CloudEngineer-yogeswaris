
# CI/CD Pipeline Architecture

## Stages

### 1. Source

* GitHub with branch protection
* Trigger: PR / push

### 2. Build

* Tool: GitHub Actions
* Run unit tests
* Coverage ≥ 80%

### 3. SAST

* Tool: SonarQube
* Block if critical issues

### 4. Dependency Scan

* Tool: Trivy
* Block critical CVEs

### 5. Integration Test

* API + DB testing

### 6. DAST

* Tool: OWASP ZAP
* Block high vulnerabilities

### 7. Compliance Gate

* Tool: OPA
* Enforce policies

### 8. Deployment

* Tool: ArgoCD
* Kubernetes deployment

## Flow

Code → Build → Scan → Test → Deploy
