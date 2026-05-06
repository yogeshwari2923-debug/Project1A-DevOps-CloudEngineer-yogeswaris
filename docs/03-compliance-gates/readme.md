
# Compliance Gates

| Gate       | Tool      | Rule            |
| ---------- | --------- | --------------- |
| SAST       | SonarQube | 0 critical      |
| DAST       | OWASP ZAP | 0 high          |
| Dependency | Trivy     | no critical CVE |
| License    | Scan      | no GPL          |
| Policy     | OPA       | K8s rules       |
| Infra      | Checkov   | no misconfig    |

## Standards

* RBI IT Risk
* PCI-DSS v4.0
