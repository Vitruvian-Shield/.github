# Decommissioned Repositories Register

This register documents repositories that have been archived or removed from the active engineering surface of Vitruvian Shield. It is maintained as an auditable record for regulatory due diligence, Series A technical due diligence and internal traceability.

Archival does not destroy history. Archived repositories remain visible in read-only form on the Vitruvian-Shield GitHub organisation for at least the minimum retention period required by our quality management system (seven years from the last commit for any repository that contributed to a regulated deliverable).

## Register

| Repository | Date archived | Reason | Successor | Archived by | Regulatory deliverables referenced |
|---|---|---|---|---|---|
| vsv1 | 2026-04-?? | Legacy PHP/Laravel web application, superseded by websiteAndSales_backend and websiteAndSales_frontend. Carries GHSA-349c-2h2t-mxf6 (laravel/passport). No patient data in scope. | websiteAndSales_backend, websiteAndSales_frontend | @paulo-martins | None |
| (populate on archival) | | | | | |

## Archival procedure

1. Open an issue in the repository tagged governance and decommission with a written decommission note referencing the successor.
2. Update this register with the date, reason, successor and approver.
3. Ensure all open pull requests are either closed, moved to the successor repository, or explicitly marked abandoned with rationale.
4. Export any regulatory deliverables (SDPs, risk analyses, traceability records) to the QMS Confluence space and record the export in this register.
5. Archive the repository via the GitHub API. Do not delete.
6. Revoke any integrations, webhooks and deploy keys associated with the repository.
7. Notify the engineering team in the Engineering Handbook space.

## Retention

Archived repositories are reviewed annually. Deletion of an archived repository requires written approval from the CTO and the Founder & CEO and must be preceded by a final export of any content referenced in the QMS.
