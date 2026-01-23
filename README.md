# APP_FORGE License Management

This repository manages license requests for APP_FORGE - Automated Application Packaging for baramundi Management Suite.

## How it works

1. **First Run**: CORE.exe generates a hardware fingerprint and creates a license request
2. **Issue Created**: Automatically submitted as GitHub Issue
3. **Grace Period**: 60 days evaluation period
4. **Approval**: DADOIT changes issue label from `pending` to `approved`
5. **Activation**: Next CORE.exe run detects approval and activates

## License Labels

| Label | Status |
|-------|--------|
| `pending` | Awaiting approval |
| `approved` | License granted |
| `revoked` | License revoked |

## Contact

- **Website**: [dadoit.ch](https://dadoit.ch)
- **Product**: APP_FORGE

---
*Copyright 2022-2026 David Dominguez - DADOIT*
