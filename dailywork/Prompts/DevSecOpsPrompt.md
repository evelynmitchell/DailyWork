```
# DevSecOps + SSDLC + AppSec Cursor Rule

## General Security Principles
- Never hardcode secrets, credentials, or API keys. Use environment variables or secure vaults for sensitive data.
- Prohibit the inclusion of `.env`, secret config files, or unknown tokens in source control.
- Never log sensitive data, secrets, or session tokens in application logs.
- Validate and sanitize all user input. Escape output in HTML, JS, and SQL contexts.
- Avoid unsafe functions such as `exec`, `eval`, or similar dynamic code execution.

## Database Security
- Use parameterized queries or ORM for all database access. Do not use string concatenation for query building.
- Ensure database users have the least privilege required for their tasks.
- Regularly review and update database access policies.

## Dependency Management
- Only use packages from verified sources.
- Do not add new dependencies without explicit approval and security review.
- Regularly update dependencies and scan for known vulnerabilities (SCA).

## Authentication & Authorization
- Use secure authentication frameworks; never implement custom authentication.
- Store passwords using strong, salted hashes (e.g., Argon2, bcrypt).
- Implement Role-Based Access Control (RBAC) for sensitive operations.
- Enforce the principle of least privilege for APIs and UI actions.

## Secure SDLC Practices
- Integrate Static Application Security Testing (SAST) and Software Composition Analysis (SCA) into the CI pipeline.
- Scan all code for secrets before merging (Secret Scanning).
- Use Infrastructure as Code (IaC) scanning for all infrastructure code.
- Integrate Dynamic Application Security Testing (DAST) in the CD pipeline for deployed applications.
- Enforce Policy as Code (PaC) for automated, version-controlled security policies.

## Monitoring & Feedback
- Enable continuous vulnerability monitoring and alerting.
- Integrate Runtime Application Self-Protection (RASP) and Web Application Firewall (WAF) as appropriate.
- Encourage regular vulnerability assessments and penetration testing.
- Maintain a feedback loop to update rules and prompts based on recurring vulnerabilities.

## Compliance & Documentation
- Align with industry standards (e.g., OWASP Top 10, NIST, ISO 27001).
- Document all security controls and decisions for auditability.
```