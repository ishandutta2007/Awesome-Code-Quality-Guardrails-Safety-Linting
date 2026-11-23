# Awesome-Code-Quality-Guardrails-Safety-Linting

<FollowUp>
Would you like to **add a dedicated section for open-source LLM prompt/output safety guardrails** (like `Llama Guard`, `NeMo Guardrails`, `LLM Guard`) or **generate the next `README.md` repository**?
</FollowUp>
# Awesome-Code-Quality-Guardrails-Safety-Linting

## Top Code Quality Guardrails & Safety Linting Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Static Analysis, Security Linting & Self-Hosted Quality Gates*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Code Quality Guardrails & Safety Linting**. These tools help teams catch bugs, security vulnerabilities, and code smells before they reach production—covering everything from commercial static analysis platforms and AI-powered PR reviewers to open-source linters and self-hosted quality gates that run entirely in your CI pipeline.

**Examples** include SonarQube, Snyk, Semgrep, ESLint, Coverity, and the emerging category of AI-agent safety guardrails (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted static analysis, open-source security linting, and community-driven quality guardrails—ideal for teams seeking to avoid per-seat or per-LOC SaaS pricing that compounds across codebases and contributors. The open-source landscape is anchored by **ESLint** (the ubiquitous JavaScript linter), **Semgrep** (lightweight pattern-based SAST), and **SonarQube Community Build** (the free, self-hosted static analysis platform).

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The static code analysis and application security testing (AST) sector is estimated at approximately **$2.0 billion to $2.2 billion (2025/2026)** and projected to exceed **$4.2 billion by 2030** (expanding at ~17–18% CAGR), propelled by rapid enterprise DevSecOps adoption and the explosion of AI-generated code. The market is **moderately concentrated (semi-consolidated)** at the top—with leading enterprise platforms (Snyk, SonarSource, Veracode, Black Duck/Coverity, and Checkmarx) capturing over 50% of total revenue—while remaining competitive and fragmented across lower-tier specialized linters and developer-first startups.

## SaaS/Hosted Platforms

| Platform | Estimated Size (Valuation / Revenue) | Pricing (Starting Tier) | Free Tier / Free Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Snyk](https://snyk.io/)** | **~$7.4B–$8.5B Valuation** (~$326M ARR) | **Team plan:** $25/month per contributing developer | **Free plan forever:** 200 Open Source (SCA) tests/mo, 100 Code (SAST) tests/mo, 300 IaC tests/mo, 100 Container tests/mo | Developer-first security scanning across code, open source dependencies, containers, and IaC configs directly in CI/CD and IDEs. |
| **[SonarQube](https://www.sonarsource.com/)** | **~$4.7B Valuation** (~$100M+ ARR) | **Team plan:** $34/month (up to 100,000 LOC) | **Free plan forever:** Up to 50,000 LOC for private projects; free without LOC limits for public open-source repos | The industry benchmark for code quality, security hot spots, and technical debt tracking across 30+ languages. |
| **[Veracode](https://www.veracode.com/)** | **~$2.5B Valuation** (~$150M–$250M ARR) | **Standard annual contract:** ~$15,000/year base (starts ~$750–$1,000/contributor/yr) | **Free trial:** 14–30 day trial with full access to SAST, SCA, and pipeline flaw analysis; no permanent free plan | Enterprise AppSec platform providing comprehensive static analysis, dynamic testing, and software composition analysis with compliance reporting. |
| **[Coverity](https://www.synopsys.com/)** | **~$2.1B Valuation** (Black Duck carve-out, ~$100M+ ARR) | **Commercial license:** Starts at ~$720/year per user (custom enterprise contracts typically starting at $15k–$25k/yr) | **Free trial:** 14–30 day sales-provisioned evaluation trial (unlimited free analysis for qualifying open-source repos via Coverity Scan) | Deep enterprise static analysis and safety-critical defect detection for C, C++, Java, C#, and other core enterprise stacks. |
| **[Checkmarx](https://checkmarx.com/)** | **~$1.15B Valuation** (~$200M+ ARR) | **Checkmarx One:** Starts at ~$30,000/year minimum platform commitment (~$1,000/developer/year for SAST) | **Free trial:** 14-day evaluation POC agreement upon sales approval (or 30-day trial for Developer Assist); no permanent free plan | Enterprise AST and ASPM suite covering static application security testing, API security, and supply chain risk management. |
| **[Code Climate](https://codeclimate.com/)** | **~$65M Raised** (~$10M–$15M ARR) | **Pro plan:** $20/contributor/month | **Free plan forever:** Unlimited analysis for public open-source repositories; 14-day free trial for private repos | Automated code review and maintainability analytics calculating test coverage, code smells, and churn metrics. |
| **[Codacy](https://www.codacy.com/)** | **~$15M Raised** (~$15M–$18M ARR) | **Team plan:** $18/contributor/month (annual billing) or $21/month (monthly) | **Developer plan forever:** $0 (IDE-only offline scanning, unlimited auto-fix, SAST & secret linting); free cloud tier for OSS | Automated code review platform supporting 50+ linters and 12,000+ rules with security and code standard enforcement. |
| **[DeepSource](https://deepsource.com/)** | **~$3M Raised** (Seed/YC, ~$2M–$5M ARR) | **Team plan:** $30/contributor/month (annual billing) | **Open Source plan forever:** $0 for public repos (unlimited members, 1,000 PR reviews/month); 14-day free trial on Team tier | Modern developer-focused static code analysis, auto-formatting, and vulnerability scanning with automated PR autofixing. |

## Open-Source GitHub Projects

- **[ESLint](https://github.com/eslint/eslint)**  
  **The ubiquitous open-source JavaScript/TypeScript linter.** **MIT licensed**, completely free [citation:6]. **Pluggable rules** for code quality, security patterns, and style. **Runs in CI** with zero licensing cost. The foundation for most JavaScript quality guardrails. **Best for any JavaScript/TypeScript project** needing reliable, configurable linting.

- **[Semgrep](https://github.com/semgrep/semgrep)**  
  **Lightweight static analysis for security and code quality.** **Open-source core** (LGPL 2.1). **Pattern-based scanning** across 30+ languages. **Fast enough to run on every commit** without slowing CI. **Rules can be written in YAML** and shared across teams. **Best for teams wanting fast, customizable SAST** that integrates easily into existing workflows.

- **[SonarQube Community Build](https://github.com/SonarSource/sonarqube)**  
  **The free, self-hosted edition of SonarQube.** **21 languages** including Java, JavaScript, TypeScript, Python, C#, Go, Ruby, PHP, Rust, Kotlin, and IaC (Terraform/Docker/Kubernetes). **Detects bugs, vulnerabilities, security hotspots, and hardcoded secrets**; tracks technical debt and code quality history. **CI/CD integration** with GitHub, GitLab, Bitbucket, and Azure DevOps; **SARIF report ingestion** for third-party tools. **50+ community plugins**. **Best for teams wanting a proven, free static analysis foundation** with no seat limits.

### Additional Strong Open-Source Options

- **agent-guardrails** — **Runtime safety guardrails for AI coding agents.** Enforces policies on agent actions (file access, shell commands, network calls) with audit logging. **Best for teams deploying autonomous agents** that need safety boundaries before production.
- **Open Policy Agent (OPA)** — **Policy-as-code engine** for enforcing guardrails across infrastructure and application configs. **CNCF graduated project**, Apache 2.0. **Best for teams wanting programmable policy enforcement** beyond static linting.
- **Trivy** — **Comprehensive scanner** for vulnerabilities, misconfigurations, secrets, and licenses across containers, code, and IaC. **Apache 2.0**. **Best for supply chain security** in CI pipelines.

**Frameworks for building custom systems**: Combine **ESLint** or **Semgrep** for fast, free linting in CI, **SonarQube Community Build** for comprehensive self-hosted analysis, and **OPA** for policy-as-code guardrails. For AI agent safety, **agent-guardrails** provides runtime enforcement.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Code quality and safety linting tools analyze source code and may access proprietary logic; enforce least-privilege repository scopes and review data handling policies before connecting external services.
- **Pricing models in this category have hidden traps that compound.** **SonarQube's free tier caps at 50k LOC**—larger private projects need the **$34/month Team plan** . **Code Climate's renewal uplifts of 5–15% are typical**—negotiate 60–90 days early to avoid automatic increases [citation:5]. **Veracode has no free tier**—only a time-limited trial [citation:7]. **Checkmarx requires a custom quote** with no published pricing [citation:8]. **Open-source options are genuinely free**: ESLint is MIT and ubiquitous [citation:6], SonarQube Community Build is free with no seat limits, and Semgrep's open-source core covers most SAST needs. **Validate whether you need managed enterprise analysis (SonarQube, Snyk, Checkmarx) or self-hosted open-source tooling (ESLint, Semgrep, SonarQube Community)** before committing.

---

**Made for engineering leaders, security engineers, and developers building quality guardrails.**  
Let's make code quality and safety linting more open, automated, and enforceable.
