# The Wild Garden

**I offer the door so you can open it.**

---

An open-source seed kit for building security, accountability, and transparency infrastructure on Cloudflare.

Built for the institutions that vendors stopped caring about: credit unions, municipalities, school districts, nonprofits, small businesses. Every one of them has the same compliance requirements as a Fortune 500. None of them have the budget. This is for them.

## What You Get

Clone this repo. Run `wrangler deploy`. You're on Cloudflare with a working framework:

- **On-prem scanning agent** — crawls file shares and databases behind your firewall
- **Cloudflare Tunnel** — outbound-only, post-quantum encrypted (X25519MLKEM768 on TLS 1.3), no firewall changes needed
- **Workers orchestration** — serverless edge compute, processes scan results in milliseconds
- **AI classification** — tiered approach: regex patterns first, LLM for ambiguous cases
- **D1 + R2 storage** — results database and evidence storage, zero egress fees
- **Examiner-ready reporting** — output mapped to compliance frameworks (NCUA, NIST CSF 2.0, ACET)

Total infrastructure cost on Cloudflare's free tier: **$0**. On paid tier for a 200-person institution: **under $10/month**.

## The Wild Garden Network (Opt-In)

The seed kit works standalone. Your data, your infrastructure, you owe nobody anything.

But if you want to be part of something bigger, there's an opt-in accountability network called the Wild Garden:

```
WILD_GARDEN = false    # default: standalone, no connection to anyone
WILD_GARDEN = true     # opt-in: join the network, your daemon goes live
```

One boolean. Off by default. On by choice.

When you opt in:
- Your daemon publishes your accountability dashboard to the network
- Other members' daemons can find you based on shared values and verified behavior
- Reputation is built on traffic patterns, not marketing budgets
- Discovery is driven by verified behavior, not purchased attention

The code is open. You can read every line. The trust is in the transparency.

## Who This Is For

- **Credit unions** that need to know where member PII lives on-prem but every vendor says "cloud only"
- **Municipalities** that want unified security visibility across departments for $7/seat
- **Nonprofits** that want to prove where every dollar goes — not with a PDF, with a live dashboard
- **Small businesses** that want to show customers they're trustworthy through verified behavior, not marketing
- **Hackers and tinkerers** who want to learn Cloudflare on the free tier with a working project to start from
- **Anyone** who believes accountability should be the default, not the exception

## The Philosophy

The hardest part of Cloudflare is the first week. Getting past the onboarding cliff — understanding Workers, Tunnels, D1, R2, Zero Trust — is what stops most people. Once you're past it, everything deploys in seconds and costs pennies.

I spent 3 weeks building 15 production applications on Cloudflare. Security dashboards, fleet management, telemetry pipelines, AI classification engines. I did the hard part so you don't have to.

The seed kit is free because the code was never the value. The value is 20 years of security architecture experience that knows what to build, why, and how to make it pass an examination. If you need that — I'm here. If you don't — build something amazing and tell your friends.

**The money isn't in the thing. It's in what you do with the thing.**

## Status

This project is in active development. The founding cohort (12 charter members) will define the governance framework before the network opens to the public.

If you want to be part of the founding table, open an issue or reach out.

## Coming Soon

- Scanning modules: data classification, certificate discovery, configuration drift, and more
- Governance framework for the Wild Garden network
- Blog post: "The Hardest Part of Cloudflare Is the First Week"
- Whitepaper: "The Wild Garden: A Cooperative Accountability Network"

---

Built by [Northwoods Sentinel](https://northwoodssentinel.com) in Madison, Wisconsin.

Infrastructure: [Cloudflare](https://cloudflare.com) (SOC 2 Type II, PCI DSS Level 1, ISO 27001, FedRAMP Moderate)

License: MIT
