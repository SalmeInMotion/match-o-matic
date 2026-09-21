# Match-o-matic Beta Privacy Notice

Effective date: 2026-09-21

## Controller and contact

Controller: **Ivan Salmeron Segovia, trading as SalmeInMotion**

Postal contact address: **Avenida del Cardenal Herrera Oria 171, 17A,
28034 Madrid, Spain**

Privacy contact: `ivan@salmeinmotion.com`

Technical support: `bugs@salmeinmotion.com`

## Why data is processed

Match-o-matic processes the minimum data needed to invite testers, deliver a
passwordless access code, start and administer the 30-day beta, enforce the
two-computer limit, refresh the seven-day offline window, prevent abuse and
answer support requests. Access administration is performed to take steps at
the tester's request and to provide the beta access arrangement. Short-lived,
in-memory IP throttling is used for service security and abuse prevention.

The Houdini activation dialog does not enrol anyone in marketing. Any future
marketing consent must be separate, optional and withdrawable without losing
beta access.

## Data used

- Normalised email address.
- Random installation identifier; the server stores only its SHA-256 hash.
- Trial start, expiry, activation, refresh and deactivation timestamps.
- Hashed one-time verification codes and bounded audit event names.
- Source IP held only in volatile memory for up to one hour for rate limiting.
- Information deliberately included by a tester in an email or GitHub issue.

No footage, Houdini scene, camera, solve, geometry, mask, production path or
licence token is uploaded by the access client or bug-report command.

## Retention

- Verification-code records: 30 days.
- Expired beta trials and activation metadata: 90 days after beta expiry.
- Access audit events: at most 120 days.
- Volatile IP-rate-limit entries: at most one hour and never written to the
  access database.
- Bug reports: while the issue is actionable, then deleted or anonymised when
  they contain personal data.
- A separately consented marketing address: until consent is withdrawn. The
  Houdini beta client does not currently collect this consent.

Retention cleanup runs automatically in the beta service. Expiry never deletes
the tester's Houdini nodes, cameras, solves, geometry or local files.

## Recipients and infrastructure

- DonDominio carries the passwordless email message.
- GitHub hosts the optional public bug tracker and release metadata when a
  tester chooses GitHub.
- The access database and signing service are hosted directly on the
  controller's own infrastructure. Cloudflare provides DNS only and does not
  proxy beta API traffic.

## Rights

Testers may request access, rectification, deletion, restriction, objection or
portability, where applicable, by writing to `ivan@salmeinmotion.com`. They may
also complain to the Spanish Data Protection Agency (AEPD):
https://www.aepd.es/

There is no automated decision-making or profiling. A refusal is limited to
the mechanical beta rules: invalid code, expired trial, offline refresh limit,
two active computers or abuse throttling.

## Changes

Material changes will be published in the public Match-o-matic repository
before they take effect.

This notice describes the beta access service as deployed on its effective
date. It is not a general privacy notice for unrelated SalmeInMotion services.
