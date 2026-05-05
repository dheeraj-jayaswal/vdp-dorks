# 🔍 vdp-dorks

> A curated collection of Google Dorks targeting publicly listed **Vulnerability Disclosure Programs (VDPs)** — for authorized reconnaissance and ethical security research only.

---

## ⚠️ Legal Disclaimer

> **Read before use.**

- All dorks in this repository are intended **strictly for use against targets that have an active, publicly listed VDP or Bug Bounty Program**.
- Using these dorks against systems **without explicit authorization** is illegal and unethical.
- The maintainer holds **no responsibility** for misuse of any content in this repository.
- Always operate within the **defined scope** of the target's VDP policy.
- This repository is for **personal reference and authorized security research only**.

---

## 📌 What is a VDP?

A **Vulnerability Disclosure Program (VDP)** is a formally published policy by an organization that:
- Invites security researchers to **find and report** vulnerabilities
- Defines the **scope** of systems that can be tested
- Provides a **safe harbor** for good-faith researchers

> Examples: HackerOne public programs, Bugcrowd public programs, company-hosted security.txt pages.

---

## 🗂️ Repository Structure

```
vdp-dorks/
│
├── reconnaissance/
│   ├── subdomain-enum.md         # Subdomain and host discovery dorks
│   ├── tech-fingerprinting.md    # CMS, framework, server detection
│   └── exposed-panels.md         # Admin, login, dashboard panels
│
├── sensitive-exposure/
│   ├── config-files.md           # Exposed configs, env files, keys
│   ├── credentials.md            # Leaked creds, tokens, API keys
│   ├── backup-files.md           # .bak, .old, .zip, .sql exposures
│   └── directory-listing.md      # Open directories and indexes
│
├── api-discovery/
│   ├── api-endpoints.md          # Exposed REST/GraphQL endpoints
│   ├── swagger-docs.md           # Swagger UI, OpenAPI spec files
│   └── postman-collections.md    # Leaked Postman collections
│
├── error-and-debug/
│   ├── error-messages.md         # Stack traces, debug info, verbose errors
│   └── dev-environments.md       # Staging, dev, test environments
│
├── cloud-and-infra/
│   ├── aws-s3.md                 # Exposed S3 buckets and objects
│   ├── gcp-azure.md              # GCP/Azure exposed resources
│   └── ci-cd.md                  # Jenkins, GitLab CI, exposed pipelines
│
├── domain-specific/
│   ├── banking-fintech.md        # Finance and banking VDP targets
│   ├── ecommerce.md              # E-commerce and retail targets
│   ├── logistics.md              # Freight and logistics targets
│   ├── education.md              # EdTech and education targets
│   └── government.md             # Government VDP targets
│
└── README.md
```

---

## 🧩 Dork Entry Format

Every dork in this repo follows a consistent format for clarity and traceability:

```
### [Dork Title]

**Dork:**
site:target.com ext:env "DB_PASSWORD"

**Purpose:**
Finds exposed .env files that may contain database credentials.

**VDP Relevance:**
High — commonly in scope for web application programs.

**Risk Level:** 🔴 Critical / 🟠 High / 🟡 Medium / 🟢 Low

**Notes:**
Refine with specific subdomains or file extensions based on target stack.
```

---

## 🏷️ Risk Level Legend

| Badge | Level | Description |
|---|---|---|
| 🔴 | Critical | Direct credential/key exposure |
| 🟠 | High | Sensitive data or config exposure |
| 🟡 | Medium | Information disclosure, recon value |
| 🟢 | Low | General fingerprinting, low sensitivity |

---

## 🎯 Scope Reminder

Before using any dork, verify:

- [ ] Target has an **active VDP or Bug Bounty Program**
- [ ] Asset is **in scope** per the program policy
- [ ] You are **not automating** queries in violation of Google ToS
- [ ] You are operating under **good faith research** principles

---

## 📚 Useful VDP Program Directories

| Platform | URL |
|---|---|
| HackerOne | https://hackerone.com/bug-bounty-programs |
| Bugcrowd | https://bugcrowd.com/programs |
| Intigriti | https://app.intigriti.com/programs |
| YesWeHack | https://yeswehack.com/programs |
| security.txt | https://securitytxt.org |

---

## 👤 Maintainer

**Dheeraj**
Certified Ethical Hacker | Web & API Penetration Tester
Domains: Banking · E-Commerce · Logistics · Education · Income Tax

---

*Last updated: May 2026*
