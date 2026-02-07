# Security Policy

## Supported Versions
This project is a **forensic analysis scaffold** and may be deployed in sensitive environments. Only the **latest tagged release** is considered supported unless your organization maintains a fork with its own support process.

If you are using a fork, please follow your internal security policy and patch cadence.

## Reporting a Vulnerability
Please **do not** open public GitHub issues for security vulnerabilities.

Instead, report privately via one of the following channels:

1) **GitHub Security Advisories**
- Use: Repository → **Security** → **Advisories** → **Report a vulnerability**
- Preferred method when enabled.

2) **Email (if you maintain it)**
- Send to: `security@YOURDOMAIN` (replace with your address)
- Subject: `SECURITY: ForensicGPT vulnerability report`

Include:
- A clear description of the issue and impact.
- Steps to reproduce (PoC preferred, but avoid weaponized exploit code).
- Affected versions/commit hash.
- Any logs, stack traces, or screenshots (redact sensitive data).
- Your suggested fix, if available.

## What to Expect
- **Acknowledgement:** We aim to acknowledge within **7 days**.
- **Triage:** We will assess severity and scope, and may request additional details.
- **Remediation:** We will work toward a fix and coordinate disclosure timing.

## Disclosure Guidelines
We follow coordinated disclosure practices:
- Avoid public disclosure until a fix or mitigation is available.
- If you believe there is active exploitation, flag this in your report.

## Security Hardening Recommendations (Deployment)
If you deploy this in production, you should:
- Place behind **SSO + MFA** (reverse proxy).
- Restrict access by network (VPN/allowlists).
- Enable encryption at rest for `/data` (evidence storage).
- Apply least-privilege filesystem permissions.
- Disable public exposure of logs and exports.
- Use separate OpenAI API keys per environment (dev/stage/prod).
- Implement rate limiting and request size limits.
- Maintain audit logs and retention policies aligned with your legal requirements.

## Out of Scope
The following are generally out of scope unless explicitly enabled by default:
- Misconfiguration in your hosting environment.
- Vulnerabilities in third-party dependencies that do not affect this project’s runtime.
- Social engineering or phishing attempts against maintainers/users.
