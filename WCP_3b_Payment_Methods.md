# WCP Browser Settings — Passwords and Autofill / Payment Methods

> **Path:** Settings → Passwords and autofill → Payment methods

---

## Tree Structure

```
Passwords and autofill
└── Payment methods
    ├── [Toggle] Save and fill payment methods (ON)
    ├── [Toggle] Save security codes (ON)
    ├── [Toggle] Allow sites to check if you have saved payment methods (ON)
    └── Payment methods [section]
        ├── [+] Add payment method → Add payment method modal
        └── [Card entry] e.g. Visa •••• 8317 · 11/29
            ├── [···] Context menu
            │   ├── Edit → Edit payment method modal
            │   └── Delete
            └── [Click row] → Edit payment method modal (Edit = View)
```

---

## 1. Payment Methods — Main Page

**Path:** Passwords and autofill / Payment methods

| Setting | State | Description |
|---|---|---|
| Save and fill payment methods | ON | Fills in payment forms with your saved payment methods. |
| Save security codes | ON | When enabled, Microsoft Copilot will securely store your security code (CVV/CVC) on this device, allowing for faster and more convenient checkout by automatically filling it in during the payment process. |
| Allow sites to check if you have saved payment methods | ON | *(highlighted row — no additional description visible)* |

| Element | Description |
|---|---|
| Payment methods [section] | Lists all saved cards with [+] Add button |
| + | Opens Add payment method modal (see §1.1) |
| [Card entry] | e.g. Visa logo · *Visa •••• 8317* · *11/29* · [···] |
| ··· | Opens context menu: Edit / Delete (see §1.2) |
| [Click card row] | Opens Edit payment method modal directly — Edit = View (see §1.3) |

---

## 1.1 Add Payment Method Modal

**Trigger:** Click **+** button in the Payment methods section header

| Field | Required | Input | Notes |
|---|---|---|---|
| Card number | ✱ | Enter card number | Hidden by default; eye-slash icon to reveal |
| Name on card | ✱ | Enter name | |
| Expiration | ✱ | [MM ▼] [YYYY ▼] | Two separate dropdowns (month / year) |
| CVV | Optional | Enter CVV | Eye icon to reveal; ⓘ info button with tooltip |
| Card nickname | Optional | Enter a nickname | |
| Billing address | Optional | Add new address [▼] | Dropdown; no address pre-filled when adding a new card |

**CVV ⓘ tooltip:**
> *"If provided, CVV will be securely stored on this device to make autofill quicker and easier.*
> *If you save your card to your Microsoft account, it will be used to authenticate your card but is not saved by Microsoft."*

**Actions:** [Save] · [Cancel]

---

## 1.2 Card Entry — Context Menu (···)

**Trigger:** Click **···** on a saved card entry

| Option | Action |
|---|---|
| Edit | Opens Edit payment method modal → §1.3 |
| Delete | Removes the saved card |

---

## 1.3 Edit Payment Method Modal (= View Card)

**Trigger:** Click a saved card entry row, OR ··· → Edit

> **Note:** There is no separate read-only "view" page. Clicking a saved card entry opens the Edit modal directly. **Edit = View.**

| Field | Required | Value | Notes |
|---|---|---|---|
| Card number | ✱ | ••••••••• [eye] | Masked; eye icon to reveal full number |
| Name on card | ✱ | [existing name] | e.g. LIU DANFENG |
| Expiration | ✱ | [MM ▼] [YYYY ▼] | e.g. 11 / 2029 |
| CVV | Optional | Enter CVV [eye] | ⓘ tooltip (same as Add modal) |
| Card nickname | Optional | Enter a nickname | |
| Billing address | ✱ | [existing address] [▼] | Required (*) when an address is already saved to this card |

> **Billing address required vs. optional:**
> In the Add modal, billing address is *optional* because no address exists yet.
> In the Edit modal, billing address becomes *required* (*) once an address has been saved.

**Billing address dropdown options:**
- • [existing address] — currently selected, e.g. *23B, Tower5,Phase1, 6 LaiYing, HONG KONG , Hong Kong SAR*
- Add new address

**Footer links:** Privacy · Copilot Terms

**Actions:** [Save] · [Cancel]

---

*Source: WCP Browser Settings screenshots — folder `3b_Payment_methods`*
*Documented: 2026-04-22*
