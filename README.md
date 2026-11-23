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
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[SonarQube](https://www.sonarsource.com/)**  
  **The enterprise standard for code quality and security analysis.** **Free tier for private projects up to 50k LOC**; **Team plan from $34/month** (up to 100k LOC); **Enterprise custom-priced** with unlimited LOC [citation:11]. **Free forever for OSS maintainers** (public, OSI-licensed repos get Pro-plan features) . Includes **SonarQube MCP Server** (open source) for AI agent integration, and **SonarQube for IDE** (free extension) for real-time analysis . Best for teams wanting a proven, comprehensive quality gate with a genuine free tier for small private projects.

- **[Snyk](https://snyk.io/)**  
  **Developer-first security with a genuine free tier.** **Free: $0/month** with SCA, SAST (Snyk Code), IaC, and Container access—limits are **200 Open Source tests, 100 Code tests, 300 IaC tests, 100 Container tests** [citation:2][citation:12]. **Team: $25/month** for increased limits. Best for development teams wanting security integrated into IDEs and CI without upfront cost.

- **[DeepSource](https://deepsource.com/)**  
  **Static analysis with a free Open Source plan.** **Open Source: $0** for public repos with unlimited members and **1,000 PR reviews/month**; AI Review and Autofix available pay-as-you-go [citation:3]. **Team: $30/month per contributor** (full features, bundled AI credits); **Enterprise custom** with self-hosted deployment and SSO [citation:13]. **14-day free trial** of Team features available [citation:13]. Best for open-source projects and small teams wanting a modern static analysis platform.

- **[Codacy](https://www.codacy.com/)**  
  **Static analysis with a free forever tier for individuals and OSS.** **Developer: $0 forever** (IDE-only, unlimited offline SAST/secrets/dependency scanning, auto-fix, MCP integration) [citation:14]. **Team: $18/dev/month annual** ($21 monthly) for up to 30 developers, 100 private repos, full cloud platform with 54 tools and 12,000+ rules [citation:14]. **Business custom** for enterprises needing DAST, container scanning, SSO, audit logs, and SBOM [citation:14]. Best for teams wanting a generous free tier and a clear upgrade path.

- **[Code Climate](https://codeclimate.com/)**  
  **Quality and velocity analytics.** **Free tier available**; **Pro: $20/contributor/month; Enterprise: $30/contributor/month** (per CostBench) [citation:15]. **Vendr data**: small teams (5–15 committers) budget **$4,000–$10,000/year** for Quality alone; mid-size (20–50) **$12,000–$35,000**; larger (75+) **$30,000–$80,000+** [citation:5]. **Renewal uplifts of 5–15% are typical**—negotiate 60–90 days early for flat or minimal increases [citation:5]. Best for teams wanting quality metrics alongside static analysis.

- **[Coverity](https://www.synopsys.com/)**  
  **Enterprise static analysis with a long pedigree.** **Pricing available upon request**; Software Advice lists starting at **$720/year** (per comparison data) [citation:9]. Positioned for large organizations with complex, safety-critical codebases.

- **[Veracode](https://www.veracode.com/)**  
  **Enterprise application security.** **No free tier** as of September 2026; **14–30 day free trial** typically available with most features [citation:7]. **8 pricing tiers** (Risk Manager, Fix, SAST, DAST, SCA, etc.) with custom pricing [citation:7]. Best for enterprises needing comprehensive AppSec with SLA-backed support.

- **[Checkmarx](https://checkmarx.com/)**  
  **Enterprise SAST and SCA.** **Checkmarx One** is priced by quote with **no published price list**; SAST is core, with Secrets, IaC, API Security, SCA, Container Scanning, and DAST as add-on modules [citation:8]. **Legacy self-hosted products** available for on-premises deployment [citation:8]. Best for large organizations needing modular AppSec coverage.

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
