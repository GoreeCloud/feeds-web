# GoreeCloud Feeds Web Security

## Current status

The repository is in Development at toolchain level. No rendered web application is currently accepted as secure, deployable, production-ready, or Stable.

Current security-relevant properties:

- no user-facing runtime or network client exists;
- no authentication/session/token storage is implemented;
- no browser-local durable user data is implemented;
- no third-party analytics or production telemetry is implemented;
- the initial TypeScript compiler dependency is pinned exactly;
- CI installs development tooling with package lifecycle scripts disabled; and
- Glaze UI, Identity, Wardveil Security, Privacy Shield, CSP/origin controls, and runtime security behavior remain acceptance-gated.

## Reporting security issues

Do not place credentials, private keys, active tokens, restricted exploit details, or private user data in public issues. Use an approved private GitHub security-reporting mechanism or another owner-approved private channel when confidential handling is required.

## Outstanding security boundaries

Future implementation must use accepted GoreeCloud Identity integration; protect sessions/tokens; avoid storing reusable secrets in source or unsafe browser storage; treat feed/article HTML and external content as untrusted; prevent injection and unsafe navigation; enforce server-side authorization rather than trusting client presentation; use Wardveil Security before production security acceptance; apply safe CSP/origin/network policies where appropriate; preserve security-relevant diagnostics without leaking content; and fail closed when authorization/security state is uncertain.

A build, test pass, or deployment does not by itself establish production security acceptance.
