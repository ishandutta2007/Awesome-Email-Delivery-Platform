# Awesome-Email-Delivery-Platform

# Top Email Delivery & Deliverability Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Transactional Email APIs, Deliverability Monitoring, DMARC Enforcement & Email Warmup*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Email Delivery & Deliverability**. These tools help developers and marketers send transactional emails at scale, monitor inbox placement, enforce DMARC policies, and warm up sending domains to maximize deliverability.

**Examples** include Mailgun, SendGrid, Postmark, Amazon SES, Resend, Brevo, DMARC Report, PowerDMARC, EasyDMARC, InboxAlly, MailReach, Warmy, and Lemwarm (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom SMTP infrastructure, and transparent deliverability tooling — ideal for teams that need full control over their email infrastructure without per-email fees or vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

### Transactional Email APIs

- **[Mailgun](https://www.mailgun.com/)**
  Developer workhorse for transactional email. Strong deliverability tooling, built-in email validation, and analytics. Free plan allows 100 emails/day; Basic $15/mo for 10,000 emails; Foundation $35/mo for 50,000; Scale $90/mo for 100,000 with SAML SSO and dedicated IP pools. Overage runs $1.10–$1.80 per 1,000. Email validation is a separate add-on .

- **[SendGrid](https://sendgrid.com/)**
  Enterprise incumbent (now part of Twilio). Combines transactional and marketing email at scale. The old free tier is gone, replaced by a 60-day trial (100 emails/day) and a permanent free tier of 100/day. Essentials starts at $19.95/mo; Pro is $89.95/mo for up to 2.5 million emails with dedicated IP, SSO, and subuser management .

- **[Postmark](https://postmarkapp.com/)**
  Premium transactional email focused exclusively on speed and reliability. Sub-second delivery times, transparent message activity showing full SMTP conversation, and deliberate exclusion of marketing blasts. Pricey at scale but the right trade for teams prioritizing transactional focus .

- **[Amazon SES](https://aws.amazon.com/ses/)**
  Raw email infrastructure at unbeatable cost: $0.10 per 1,000 emails. New AWS accounts get up to 3,000 message charges free per month for the first 12 months. Dedicated IPs are $24.95/mo standard, or a managed option at $15/mo plus per-message fee. Requires engineering capacity to build templates, handle reputation, and monitor deliverability .

- **[Resend](https://resend.com/)**
  Developer-focused platform designed for modern web frameworks (Next.js, Remix). First-class React Email integration allows coding responsive templates with React components. Clean DX and minimalist documentation. Founded 2022, shorter enterprise track record. Free tier: 3,000 emails/month (100/day limit). Paid starts at $20/month for 50,000 emails .

- **[Brevo](https://www.brevo.com/)**
  All-in-one platform combining transactional email with marketing, SMS, WhatsApp, and CRM. Free plan includes 300 daily email sends. Good fit when one team needs both application emails and broader customer messaging .

- **[MailerSend](https://www.mailersend.com/)**
  Budget pick from the team behind MailerLite. Bundles a genuinely good drag-and-drop template builder with transactional sending, plus SMS. Strong value for teams needing polished templates without enterprise pricing .

### DMARC & Email Authentication

- **[DMARC Report](https://dmarcreport.com/)**
  Enterprise-grade DMARC reporting with aggregate and forensic analysis. G2 rating: 4.8/5 (458 reviews). Visual dashboards, source classification by vendor, multi-domain management, MSP partner program. SOC-2 Type II, signed SLAs, SSO/SAML, RBAC. Free (10K reports, 1 domain) → Guard $25/mo → Shield $75/mo → Defender $200/mo → Ultimate $345/mo. SPF management via sister product AutoSPF .

- **[PowerDMARC](https://powerdmarc.com/)**
  Full-stack email authentication platform. All-in-one dashboard covering DMARC, SPF, DKIM, BIMI, MTA-STS, TLS-RPT with AI-powered threat intelligence. 10,000+ organizations across 100+ countries. Free plan: 10,000 compliant emails/month; Basic from $12/mo. Strong value play for teams needing broad protocol coverage .

- **[EasyDMARC](https://easydmarc.com/)**
  User-friendly DMARC platform with guided onboarding. Intuitive dashboard, smart DNS scanning, one-click Cloudflare setup, sender identification by name. Free tier: 1,000 emails/month, 1 domain, 14 days history. Plus at $44.99/mo (or $35.99/mo annually) for small teams wanting a real dashboard without enterprise pricing .

- **[dmarcian](https://dmarcian.com/)**
  DMARC visibility and reporting pioneer. Clear, visual reporting with graphical SPF surveyor, strong educational content. Focuses on helping organizations understand their DMARC data before enforcing. Best for teams early in their DMARC journey who want reporting clarity first .

- **[Valimail](https://www.valimail.com/)**
  Enterprise DMARC automation (now part of DigiCert). Automated SPF/DKIM management, zero-DNS-maintenance approach, "Monitor → Enforce → Align" journey structure. Service identification by name as first-class feature. Large enterprises wanting automated DMARC enforcement with minimal manual DNS work .

- **[Red Sift OnDMARC](https://redsift.com/)**
  MSP-focused DMARC platform. Purpose-built multi-tenant platform with API-first architecture, Dynamic SPF technology, flat-rate MSP pricing. MSPs and MSSPs managing multiple client domains needing API-driven automation .

- **[Postmark DMARC Digests](https://postmarkapp.com/dmarc)**
  Best "I'll actually read it" option. Digest, not a dashboard — free weekly email covering top 10 mail sources with 7 days history. Paid tier ($14/mo per domain) adds all sources, web dashboard, and 60-day history. Suits single-domain operators wanting a small paid dashboard .

### Email Warmup & Deliverability

- **[InboxAlly](https://inboxally.com/)**
  Best for advanced engagement-based email warmup and reputation recovery. No peer network — sends to controlled seed accounts that open, read, flag as important, and take out of spam. Works with any email provider. Custom warmup strategies and real-time inbox reports. Pricing from $149/mo (Starter) to $1,190/mo (Premium). Best for senders whose emails land in spam and need reputation recovery .

- **[MailReach](https://www.mailreach.co/)**
  Reputation monitoring and warming with detailed spam-placement reports. Published pricing with a slider: one mailbox with 20 spam test credits comes to €25/mo, with per-mailbox rate decreasing at scale. Closest direct swap for Warmy.io .

- **[Warmy](https://warmy.io/)**
  AI-powered warmup with analytics. Two separate warming networks: one on business mailboxes (Google Workspace, Microsoft 365), another on consumer accounts (Gmail, Yahoo, Outlook). You pick the one matching your audience. Pricing from $49/mo per mailbox. Billing model per-mailbox becomes the highest recurring cost as you add inboxes .

- **[Lemwarm](https://www.lemlist.com/)**
  Built-in warmup for Lemlist users. Real-time inbox placement tracking, custom warmup scenarios, smart recommendations based on domain reputation. Seamless integration with Lemlist outreach. Pricing from $24/mo per email .

- **[Warmup Inbox](https://warmupinbox.com/)**
  Budget-friendly automated email warmup. Simple deliverability dashboard, domain and IP reputation improvement. Plans from $15–$19/mo. Best for solo founders and SMBs managing one or two inboxes .

## Open-Source GitHub Projects

### Email Infrastructure & MTAs

- **[Maddy Mail Server](https://github.com/foxcpp/maddy)**
  All-in-one mail server that implements SMTP (both MTA and MX) and IMAP. Replaces Postfix, Dovecot, OpenDKIM, OpenSPF, and OpenDMARC with a single daemon. Composable-first design, single binary, automatic TLS via Let's Encrypt. GPL-3.0, Go-based. Designed to be operational in minutes rather than days .

- **[Postfix](https://github.com/vdukhovni/postfix)**
  The de facto standard for Linux mail servers. Ubiquitous, rock-stable, well-documented. Best as a mail transfer agent (receiving/proxy) rather than a high-volume sender. Configuration syntax is human-readable with English-like sentence structure .

- **[OpenSMTPD](https://github.com/OpenSMTPD/OpenSMTPD)**
  Free implementation of server-side SMTP protocol from the OpenBSD team. Focuses on simplicity and security auditability. Configuration syntax is clean and readable. Lightweight, minimal system resources. Strong choice for smaller deployments where Postfix complexity is unnecessary .

- **[KumoMTA](https://github.com/KumoMTA/KumoMTA)**
  Modern successor to PowerMTA, built by the team that created PowerMTA. Written in Rust for performance and memory safety. Handles 10M+ messages/hour on commodity hardware. Granular bounce handling, detailed per-message logging, commercial support available. Use when sending transactional email at scale (100K+/day) .

- **[Haraka](https://github.com/haraka/Haraka)**
  High-performance SMTP server written in Node.js. Excellent plugin architecture. Scales well but complex to operate at very high volume .

- **[Mailcow](https://github.com/mailcow/mailcow-dockerized)**
  Industry standard for containerized email deployments. Bundles Postfix, Dovecot, Nginx, PHP, MariaDB, and Rspamd into a cohesive Docker Compose stack. Resource-heavy but effective for those avoiding manual configuration .

### Email Verification

- **[validate-emails](https://github.com/centminmod/validate-emails)**
  Self-hosted email verification script to clean up invalid email address lists. Supports various commercial verification provider APIs all in one script. According to ZeroBounce, email lists decay by an average of 25.74% yearly, with leading causes being invalid and catch-all addresses .

- **[OmniEmailVerifier](https://github.com/topics/email-verifier)**
  Open-source platform connecting multiple email verification providers in one interface. Manages API keys and credits, routes verification requests intelligently, verifies single or bulk emails, imports TXT/CSV/XLSX files, organizes lists, filters results, and tracks history .

### DMARC Parsing & Analysis

- **[parsedmarc](https://github.com/domainaware/parsedmarc)**
  Python package and CLI for parsing aggregate and forensic DMARC reports. ~1,017 stars, actively maintained (updated this week as of search). Extensive output options including Elasticsearch, OpenSearch, Splunk, Kafka, and PostgreSQL. Supports IMAP, Maildir, and local file inputs. Production-grade with archive directory management, batch processing, and retry logic .

- **[Open DMARC Analyzer](https://github.com/techsneeze/dmarcts-report-parser)**
  PHP parser, viewer, and summary report generator for incoming DMARC reports. View parsed reports in a table with color-coded issues, filter by domain/month/reporting organization, password-protected web interface, process reports from mailboxes or local directories, generate weekly/monthly summaries. Available in Debian repositories .

- **[@domaincanary/dmarc-rua](https://jsr.io/@domaincanary/dmarc-rua)**
  DMARC RUA aggregate report parser and MIME attachment extraction library for TypeScript. Runs on Deno, Node.js, Bun, and Cloudflare Workers. Tolerates malformed records with bounded decompression and record budgets to prevent zip bombs. Parses XML, gzipped XML, and zip payloads, surfaces SPF/DKIM results and policy override reasons .

- **[dmarcts-report-parser](https://github.com/techsneeze/dmarcts-report-parser)**
  Perl-based DMARC report parser that stores reports in MySQL/MariaDB. Command-line tool for automated ingestion. Companion to the PHP viewer .

### Email Sending Libraries & Frameworks

- **[Nodemailer](https://github.com/nodemailer/nodemailer)**
  The standard email sending library for Node.js. Provider-agnostic SMTP transport with support for OAuth2, DKIM signing, and attachments. Foundation for many higher-level email frameworks.

- **[PHPMailer](https://github.com/PHPMailer/PHPMailer)**
  The classic PHP email library. SMTP with authentication, TLS/SSL, attachments, HTML/plain-text alternatives. The recommended replacement for PHP's built-in `mail()` function, which often fails silently on shared hosting due to MTA restrictions .

- **[MailWiz](https://github.com/apilayer/mail-wiz)**
  Email verification devtool powered by the Mailboxlayer API. Paste a single address, comma-separated list, or CSV — get back syntax validation, MX records, live SMTP check, catch-all detection, role/disposable/free flags, and a 0–1 deliverability score. Results export back out as CSV .

### Warmup & Outreach Platforms

- **[Emareach](https://github.com/ritik-prog/emareach)**
  Production-grade open-source AI email marketing platform with automation, campaigns, deliverability, analytics, and self-hosting. Features mailbox warmup with LLM-generated threads, spam-to-inbox recovery, SPF/DKIM/DMARC checks, multi-step campaigns, contact enrichment, and smart lead search. FastAPI backend, Next.js frontends, MongoDB, Docker Compose, Terraform for AWS. Apache-2.0 .

- **[Warmbly](https://www.producthunt.com/products/warmbly)**
  Open-source platform for modern cold outreach with AI automations, real-time collaboration, agents, and email warmup. Free. Early-stage but supports campaigns, warmup, automations, analytics, and team collaboration. Working on hosted version and mobile app .

### Additional Strong Open-Source Options

- **Self-Hosted Email Suites**: **Mail-in-a-Box** (one-click email server setup), **iRedMail** (full-featured email server), **Mailu** (Docker-based email server), **docker-mailserver** (production-ready containerized mail server).
- **SMTP Testing**: **MailHog** (email testing for developers), **Mailpit** (modern email testing tool), **smtp4dev** (SMTP server for testing).
- **Email Templates**: **MJML** (responsive email framework), **Maizzle** (Tailwind CSS for emails), **React Email** (React components for email templates).
- **Deliverability Monitoring**: **Postfix Exporter** (Prometheus metrics from Postfix logs), **Rspamd** (spam filtering with statistics).

**Frameworks for building custom systems**: Combine **Maddy Mail Server** for all-in-one SMTP/IMAP with built-in DMARC analysis, **parsedmarc** for DMARC report ingestion and analysis, **KumoMTA** for high-volume transactional sending, and **Emareach** for warmup and outreach automation. Add **Mailcow** for containerized mail infrastructure and **PHPMailer** or **Nodemailer** for application-level sending.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Email delivery platforms handle sensitive communications; ensure compliance with CAN-SPAM, GDPR, and relevant anti-spam regulations.
- **Open-source reality**: Self-hosted email infrastructure is technically mature (**Maddy**, **Postfix**, **KumoMTA**) but carries significant hidden costs. A production-grade MTA stack requires at least 2GB RAM VPS (~$10–20/mo), plus engineering hours for reputation management, IP warmup (30–60 days), log analysis, and security patching. IPs from commodity cloud providers are frequently blocklisted, and cleaning them can take weeks. The software is free; the operational burden is substantial .

---

**Made for developers, email infrastructure engineers, deliverability specialists, and marketing operations teams.**
Let's make email delivery more open, transparent, and deliverable.
