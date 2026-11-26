# Security Policy

CyberVerse is intended to become a platform involving user accounts, learning progress, AI integrations, and potentially sensitive application data. Security issues should be handled carefully.

## Reporting a vulnerability

Please do not disclose exploitable vulnerabilities, credentials, personal data, or attack instructions in public issues.

Use GitHub's private vulnerability reporting feature for this repository when it is enabled. Otherwise, contact the repository owner privately through a trusted channel and include:

- A concise description of the affected component
- Impact and realistic attack conditions
- Minimal reproduction steps or a safe proof of concept
- Relevant versions, commit, or environment
- Any suggested mitigation

Do not access, modify, download, or expose another person's data while investigating.

## Sensitive data

Never commit:

- API keys, OAuth client secrets, access tokens, or passwords
- Supabase service-role keys or database credentials
- Private certificates or signing keys
- Production environment files
- Personal data, database dumps, or real user records

Use local environment variables and appropriately scoped secret management. If a secret is exposed, revoke or rotate it immediately; deleting it from the latest commit alone is not sufficient.

## Security review expectations

The Phase 1–10 audit should examine, where applicable:

- Authentication and session handling
- Authorization boundaries and ownership checks
- Supabase Row Level Security policies and privileged server access
- Input validation, output encoding, and injection risks
- CSRF, XSS, SSRF, and unsafe file handling
- AI prompt/data boundaries, provider credentials, and abuse controls
- Rate limits, token budgets, and resource exhaustion
- Logging, error messages, and sensitive-data exposure
- Dependency and build supply-chain risks

Actual findings must be tied to inspected code or test evidence. This policy does not imply that these controls have already been implemented or verified.
