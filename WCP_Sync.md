# WCP Browser Settings — Sync and import / Sync

> **Path:** Settings → Sync and import → Sync

---

## Tree Structure

```
Sync and import
└── Sync
    ├── [Toggle] Passwords            (Default OFF)
    ├── [Toggle] Payments using Microsoft account  (Default ON)
    └── [Toggle] Personal info        (Default OFF)
```

---

## 1. Sync — Main Page

**Path:** Sync and import / Sync

**Page description:** Sync all your browsing data between Copilot apps and Edge across your signed-in devices.

### Toggle defaults

| Toggle | Default state | Controls |
|---|---|---|
| Passwords | **OFF** | 3A · Microsoft Password Manager |
| Payments using Microsoft account | **ON** | 3B · Payment Methods |
| Personal info | **OFF** | 3C · Addresses and More |

### Toggle descriptions

| Toggle | Description |
|---|---|
| Passwords | Stored securely and made available on all your devices. *Review security settings* to help make your Microsoft account even more secure. |
| Payments using Microsoft account | Cards saved in Microsoft account will be available to use across signed in devices and Microsoft products. Manage these cards in your *Microsoft account*. |
| Personal info | Information like name, date of birth, address and more are saved so online forms are filled automatically. |

---

## Design note — Compliance implication

> **Because Password Sync and Personal Info Sync are default OFF, the Sync entry point must be prominently accessible.**
> If users cannot easily find the Sync page to turn these on, compliance requirements will not be met.

---

*Source: WCP Browser Settings screenshots — folder `2_Syncsetting`*
*Documented: 2026-04-23*
