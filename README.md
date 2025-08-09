Marketplace Content Auditor — Web Scraping + Data Quality Automation
Concise version

Built a web scraping and validation system to compare marketplace PDP content (titles, bullets, specs, images, price) against the source catalog, auto‑flagging inconsistencies and missing attributes.

Stack: Python, Requests, BeautifulSoup/lxml, rotating proxies, pandas, Great Expectations/dbt tests, MySQL/BigQuery, Airflow for orchestration, Power BI/Tableau for issue tracking.

Impact: Automated content audits across thousands of SKUs, cut reconciliation time by 80%, and improved listing accuracy and conversion drivers (title relevance, image compliance, feature completeness).

Detail/impact version

Scope: Monitored top marketplaces and key PDP fields (title, description, attributes, brand, pack size, compliance tags, images, price/fees) against PIM/MDM “source of truth.”

Pipeline: Scheduled crawlers with dynamic waits and anti‑bot handling; normalized HTML to structured JSON; fuzzy‑matched attributes; applied validation rules (regex, ranges, allowed vocab); logged deltas and severity.

Governance: Great Expectations checks, SLA alerts for high‑impact SKUs, and a triage dashboard that routes issues to content ops with auto‑generated fix suggestions sourced from the master catalog.

Results: 80% reduction in manual content QA, material lift in attribute completeness, and fewer listing suppressions/penalties due to non‑compliant content.

