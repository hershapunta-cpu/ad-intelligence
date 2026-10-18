# Ad Intelligence

Ad Intelligence is the research and campaign-intelligence component of the ReBoRn ecosystem. It is intended to support evidence-based advertising research, audience insights, creative recommendations, campaign planning, client review, and reporting.

## Project status

**Foundation repository — implementation in progress.**

This repository is not yet a production-ready application. Do not treat features as live until their code, data connections, and tests have been implemented and verified.

## Intended first release

- Client-safe dashboard structure
- Advertising research and insight summaries
- Creative/ad-variant recommendations with rationale
- Campaign and project records
- Client approvals and feedback
- Performance summaries only when verified performance data is available

## Architecture principles

- Reuse the existing ReBoRn infrastructure where appropriate.
- Use the existing Supabase project; do not create duplicate projects or tables without reviewing the current schema first.
- Keep client data private and enforce organization/client access controls in the backend, not only in the interface.
- Never commit passwords, API secrets, service-role keys, access tokens, or real client confidential data.
- Clearly distinguish verified data from generated recommendations and placeholder content.
- Make small, reviewable changes and test before deploying.

## Deployment

The hosting target and deployment configuration must be confirmed before connecting this repository to a production Cloudflare project. Do not deploy this repository to a live client URL until authentication, access policies, and the intended user experience have been tested.

## Development notes

Before implementation, review the existing ReBoRn/Supabase schema and current Cloudflare projects. Document required environment variables by name only; store their values in the hosting provider's secret settings, never in source control.

## License

No license has been specified yet.
