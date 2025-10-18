# report-templates

A small collection of polished report templates and a README to help you produce professional, recruiter-friendly vulnerability assessment reports and executive summaries. This repository is intentionally sanitized and focuses on delivering clean templates you can populate with authorized lab data.  

**templates/technical-report.md** — a full, polished technical report template (markdown) you can edit and convert to PDF.  

**templates/executive-summary.md** — concise 1-page executive summary template.  

**templates/sample-findings.md** — sanitized, non-actionable finding entries and severity matrix.  

## usage & quick start  

1. Copy the templates/ folder into your new repo or use this repo as a template on GitHub.

2. Fill templates/technical-report.md with your sanitized evidence (screenshots only, no exploit payloads).

3. Convert to PDF locally using pandoc or export from your editor (instructions below).  

## How to export PDF locally  

With Pandoc (recommended for highest control):  
```
# install pandoc (if not installed)
# Debian/Ubuntu: sudo apt install pandoc
# Windows: install from https://pandoc.org

pandoc templates/technical-report.md -o report.pdf --pdf-engine=xelatex
```  

**From VSCode:** open the technical-report.md, then use the Markdown preview → Print to PDF.  

**From GitHub:** use GitHub Pages or render in a PR and print, but double-check all redactions first.  

## Sanitation & ethics reminder

Do not include exploit payloads, webshell binaries, VM images, or exact commands.

Redact IPs, hostnames, usernames, and any unique identifiers before publishing.

Keep original evidence offline and encrypted.
