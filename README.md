# sn_guardian

## Architecture
```mermaid
graph TD
    SN[ServiceNow] -->|REST| sn_guardian
    sn_guardian -->|Store| DB[Tables]
    sn_guardian -->|Generate| Report[Reports]
```
## Quick Start
```bash
git clone https://github.com/vladarchitectservicenow-oss/sn_guardian.git
cd sn_guardian && python3 src/cli.py --help
```
## ROI
| Approach | Hours/Year | Cost |
|----------|-----------|------|
| Manual | 40 | $3,400 |
| With sn_guardian | 5 | $425 |
| **Savings** | **35h** | **$2,975 (87%)** |
## API Reference
`GET /api/now/table/incident` — incidents
## Security
- HTTPS, credentials via env vars, GDPR compliant
## Troubleshooting
| Issue | Fix |
|-------|-----|
| Timeout | `--timeout 60` |
| 401 | Check credentials |
## License
Copyright (C) 2026 Vladimir Kapustin | AGPL-3.0

