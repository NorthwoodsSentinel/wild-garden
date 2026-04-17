# Security Policy

Wild Garden is a security-positioned project. We take security disclosures seriously and want to make it easy for you to report responsibly.

## Supported Versions

This repository is in **design and specification phase**. There is no deployable code yet. Once the seed kit ships, this section will list which versions receive security updates.

For now, security disclosures should focus on:
- Architectural weaknesses in the design specification
- Pattern recommendations that would introduce vulnerabilities if implemented as written
- Threat model gaps in the proposed cooperative network design

## Reporting a Vulnerability

**Please do not file public GitHub issues for security disclosures.** Use the channels below instead.

### How to Report

1. **GitHub Security Advisories** (preferred) — use the [private vulnerability reporting feature](https://github.com/NorthwoodsSentinel/wild-garden/security/advisories/new) on this repository.
2. **Email** — send to `security@northwoodssentinel.com` (set up forthcoming; until then, contact [@NorthwoodsSentinel](https://github.com/NorthwoodsSentinel) directly via GitHub).

### What to Include

- A description of the vulnerability or concern
- The location in the spec or (when applicable) the code
- Reproduction steps if relevant
- Suggested mitigation if you have one
- Your name/handle if you want recognition (anonymous reports also accepted)

### Response Commitment

- **Acknowledgment within 48 hours** — we'll confirm receipt and start triage
- **Initial assessment within 7 days** — severity, scope, planned response
- **Coordinated disclosure** — we'll work with you on timing for public disclosure

## Disclosure Philosophy

Wild Garden is built for institutions that have been told to "wait for the vendor." Our security posture should reflect that. We commit to:

- **Transparency** — when we fix a security issue, we explain what it was and why it mattered
- **Credit** — reporters who want to be named are listed in [CONTRIBUTORS.md](./CONTRIBUTORS.md) and the security advisory
- **No legal threats** — good-faith security research is welcome. We will not pursue legal action against researchers who follow this policy.
- **Responsible disclosure timing** — we'll coordinate disclosure timing with you. Default: 90 days after initial report, adjustable based on severity and complexity.

## Scope

**In scope:**
- This repository (NorthwoodsSentinel/wild-garden) — design spec, governance, patterns
- Future seed kit code (when published)
- Anything we publish under the Wild Garden name on Cloudflare

**Out of scope:**
- Third-party dependencies (report to those projects directly)
- Wild Garden member deployments of the seed kit (those are member-operated)
- Cloudflare platform issues (report to Cloudflare directly via [their HackerOne program](https://hackerone.com/cloudflare))

## Security Principles

The Wild Garden architecture itself rests on these security principles. If you're proposing changes that violate them, please flag the trade-off explicitly:

1. **Outbound-only** — agents on member networks initiate connections. No firewall holes.
2. **Post-quantum encrypted** — Cloudflare Tunnel defaults
3. **Open source** — every line readable, no security-through-obscurity claims
4. **Transparent operations** — what flows through the network is logged and accountable to members
5. **Per-member isolation** — one member's compromise should not put others at risk

---

*Reporting a vulnerability is a contribution. Thank you.*
