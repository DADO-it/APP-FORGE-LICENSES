# 🔐 APP_FORGE License Server

**Hardware-bound license management for APP_FORGE**

---

## 📁 Structure

```
APP-FORGE-LICENSES/
├── approved/           # Activated licenses
│   └── {fingerprint}.json
├── pending/            # Awaiting approval
│   └── {fingerprint}.json
└── revoked/            # Revoked licenses
    └── {fingerprint}.json
```

---

## 🔑 License Flow

1. **Customer installs APP_FORGE**
2. **CORE.exe generates 6-factor hardware fingerprint**
3. **60-day grace period starts**
4. **Customer contacts DADOIT for activation**
5. **DADOIT creates license file in `/approved/`**
6. **CORE.exe validates → Full license active**

---

## 📋 License File Format

```json
{
  "fingerprint": "ABC123...",
  "company": "Customer Name",
  "contact": "admin@customer.com",
  "activated": "2025-01-06T12:00:00Z",
  "expires": null,
  "notes": "Permanent license"
}
```

---

## 🛡️ Hardware Fingerprint (6 Factors)

1. Machine Name
2. Domain Name
3. OS Version
4. Processor Count
5. System Directory
6. APP_FORGE Install Path

---

© 2022-2025 DADOIT - All rights reserved
