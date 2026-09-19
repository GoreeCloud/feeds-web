# GoreeCloud Feeds Web Security

## Current status

This repository is in Planned / repository-foundation state. No web application is currently accepted as secure, deployable, production-ready, or Stable.

## Reporting security issues

Do not place credentials, private keys, active tokens, restricted exploit details, or private user data in public issues. Use an approved private GitHub security-reporting mechanism or another owner-approved private channel when confidential handling is required.

## Planned security boundaries

Future implementation must use accepted GoreeCloud Identity integration; protect sessions/tokens; avoid storing reusable secrets in source or unsafe browser storage; treat feed/article HTML and external content as untrusted; prevent injection and unsafe navigation; enforce server-side authorization rather than trusting client presentation; use Wardveil Security before production security acceptance; apply safe CSP/origin/network policies where appropriate; preserve security-relevant diagnostics without leaking content; and fail closed when authorization/security state is uncertain.

A build, test pass, or deployment does not by itself establish security acceptance.
