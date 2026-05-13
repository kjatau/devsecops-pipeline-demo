# DevSecOps Pipeline Demo

Automated security scanning pipeline that runs on every code push.
Catches vulnerabilities before they reach production.

## What it does
- Scans Python code for security issues using Bandit
- Checks dependencies for known CVEs using Safety
- Runs automatically on every push and pull request

## Real findings caught
- Bandit: Detected hardcoded bind to all interfaces (B104) — fixed
- Safety: Detected Flask CVE-2026-27205 — upgraded to 3.1.3

## Tools used
- GitHub Actions
- Bandit (SAST)
- Safety (dependency scanning)
- Python / Flask