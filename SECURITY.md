# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| Older   | :x:                |

We recommend running the latest release of HttpForge. Security fixes are not backported to unsupported versions.

## Reporting a Vulnerability

If you discover a security vulnerability in HttpForge, please report it responsibly. **Do not** open a public GitHub issue for security-sensitive reports.

Email: **httpforge@outlook.com**

Please include:

- A description of the vulnerability and its potential impact
- Steps to reproduce the issue
- Affected versions, if known
- Your contact information for follow-up

We aim to acknowledge reports within 48 hours and provide a remediation timeline within 7 business days.

## Our Security Model

HttpForge is a **local-first** API client:

- Credentials, environment variables, and request data are stored on your device
- We do not operate cloud servers that store your API secrets
- Requests are sent directly to the endpoints you specify — HttpForge does not proxy or log your API traffic
- Sensitive values are masked in the UI by default

For full details, see [httpforge.com/security.html](https://httpforge.com/security.html).

## Website Security Headers

The httpforge.com website uses `_headers` to serve:

- `Content-Security-Policy`
- `Strict-Transport-Security`
- `X-Frame-Options`
- `X-Content-Type-Options`
- `Referrer-Policy`
- `Permissions-Policy`

CSP and Referrer-Policy are also set via HTML meta tags on every page as defense in depth.
