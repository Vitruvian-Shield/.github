# Security Policy

Vitruvian Shield Holding SA operates regulated Software as a Medical Device and processes Special Category personal data under GDPR Article 9. Security vulnerabilities are treated as patient-safety and regulatory-compliance events, not only technical bugs.

## Supported versions

We issue security patches for the current major version and the prior major version of each published service. Older versions receive end-of-life notices and are not patched.

## Reporting a vulnerability

Do not open a public issue for suspected vulnerabilities. Instead, send a detailed report to security@vitruvianshield.com encrypted with our PGP key (fingerprint published on the corporate website). Include:

- A clear description of the issue and the affected component
- A minimal reproduction path
- The versions you tested
- Your assessment of impact (confidentiality, integrity, availability, patient safety)
- Whether you believe the issue is being actively exploited

We acknowledge reports within two business days and commit to a remediation plan within ten business days for High and Critical severity. We honour responsible disclosure and will coordinate public disclosure with you after a fix is deployed.

## Scope

In scope: all repositories under the Vitruvian-Shield GitHub organisation, all production endpoints under vitruvianshield.com and subdomains, mobile applications published under Vitruvian Shield Holding SA.

Out of scope: third-party services we integrate with (Dexcom, Corsano, Azure), marketing copy, findings that require physical access to a user device, denial of service via volumetric attack, reports of missing security headers without a demonstrable exploit.

## Severity classification

We classify using CVSS 3.1 plus a patient-safety qualifier derived from IEC 62304 software safety classification. A vulnerability in a Class C component that affects dosing, consent or audit trail integrity is treated as Critical regardless of base CVSS.

## Regulatory links

- ISO 27001:2022 Annex A controls: 8.8, 8.9, 8.15, 8.24, 8.25, 8.28, 8.29
- IEC 62304:2015 clause 5.5, 7.3, 8.2
- 21 CFR Part 11 §11.10(a), §11.10(d), §11.10(e)
- GDPR Articles 32, 33, 34
- NIS2 Directive Article 21

## Internal contacts

Security lead: Vahid Khazaei Nezhad, CTO, vahid@vitruvianshield.com.
Data Protection Officer: appointed per GDPR Article 37, dpo@vitruvianshield.com.
