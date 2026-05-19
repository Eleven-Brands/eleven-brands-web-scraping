# eleven-brands-web-scraping

Web scraping utilities and scripts for Eleven Brands. This repository collects scrapers and data extraction scripts for external data sources that are not available via official APIs.

> **Status:** Early-stage — source code is being developed. The infrastructure (CI/CD, standards sync, linting) is in place.

---

## Intended Scope

Scripts in this repo are responsible for:
- Extracting product, competitor, and market data from e-commerce platforms and public web sources
- Outputting structured data (CSV or BigQuery) for downstream analytics pipelines
- Running on a scheduled basis or triggered manually

Each scraping target will have its own subfolder following this pattern:

```bash
scrapers/
└── <target_name>/
    ├── main.py           # Entry point
    ├── config.py         # URLs, selectors, output paths
    ├── README.md         # Target-specific documentation
    └── requirements.txt  # Dependencies
```

---

## Getting started

Set up your local environment and GCP credentials by following [setup_local_development.md](setup_local_development.md) and [setup_gcp.md](setup_gcp.md).

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for the Git workflow, code style, commit conventions, and PR process.
