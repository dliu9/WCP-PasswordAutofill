# WCP Browser Settings — Passwords and Autofill / Addresses and More

> **Path:** Settings → Passwords and autofill → Addresses and more

---

## Tree Structure

```
Passwords and autofill
└── Addresses and more
    ├── [Toggle] Save and autofill addresses (ON)
    ├── [Toggle] Use AI to improve autofill suggestions (ON)
    └── Addresses [section]
        ├── [+] Add address → Add address modal         (when addresses exist)
        ├── [🗑] → Bulk delete flow                      (when addresses exist)
        ├── [···] Section menu
        │   ├── →| Import addresses (DISABLED — not implemented)
        │   └── |→ Export addresses → File save dialog
        ├── [Add address] button → Add address modal    (empty state only)
        └── [Address entry] e.g. lauda
            └── [···] Per-entry menu
                ├── Edit → Edit address modal
                └── Delete → Delete address? confirmation modal
```

---

## 1. Addresses and More — Main Page

**Path:** Passwords and autofill / Addresses and more

| Setting | State | Description |
|---|---|---|
| Save and autofill addresses | ON | Saves your name, phone number, email address, and delivery information to autofill it when you need it. |
| Use AI to improve autofill suggestions | ON | Allow Copilot to process autofill entries and field descriptions to get better autofill suggestions. Your personal data is secure and will not be used elsewhere. |

### Addresses section header — state-dependent buttons

| State | Buttons shown |
|---|---|
| No addresses (empty) | [···] only |
| Has saved addresses | [+] [🗑] [···] |

### Empty state

| Element | Description |
|---|---|
| Message | "Saved addresses will appear here" / "No addresses saved" |
| [Add address] button | Same trigger as [+] — opens Add address modal (see §1.1) |

### With saved addresses

| Element | Description |
|---|---|
| [+] | Opens Add address modal (see §1.1) |
| [🗑] | Enters bulk selection/delete mode (see §1.5.2) |
| [···] | Opens Import / Export section menu (see §1.2) |
| Address entry | Person icon · **Name** · Summary line (phone, email, street…) · [···] |
| Per-entry [···] | Opens Edit / Delete context menu (see §1.3) |

---

## 1.1 Add Address Modal

**Trigger:** [+] in section header, OR [Add address] button in empty state

All fields are optional — no asterisks shown.

| Field | Placeholder / Default | Notes |
|---|---|---|
| Country/region | United States [▼] | Dropdown |
| Name | Enter name | |
| Organization | Enter organization | |
| Street address | (empty) | |
| City | (empty) | |
| State | (empty) | |
| ZIP code | (empty) | |
| Phone | Enter phone number | |
| Email | Enter email address | |

> *"You can use saved addresses across Microsoft services. This info will be saved in your Microsoft Account."*

**Actions:** [Add] · [Cancel]

---

## 1.2 Section Header ··· Menu

**Trigger:** Click **···** in the Addresses section header

| Option | State | Notes |
|---|---|---|
| →\| Import addresses | Disabled | Feature not yet implemented |
| \|→ Export addresses | Active | Opens file save dialog → §1.2.1 |

---

## 1.2.1 Export Addresses — File Save Dialog

**Trigger:** Section ··· → Export addresses

| Element | Value |
|---|---|
| Window title | Save As |
| Default file name | `Microsoft_Copilot_Forms_YYYY_MM_DD.json` *(date-stamped)* |
| Save as type | JSON File (*.json) |
| Actions | [Save] [Cancel] |

> **Note:** Export format is **JSON** — different from passwords (CSV) and payment methods.

---

## 1.3 Per-Entry ··· Context Menu

**Trigger:** Click **···** on a saved address entry row

| Option | Action |
|---|---|
| ✏️ Edit | Opens Edit address modal → §1.4 |
| 🗑 Delete | Opens Delete confirmation modal directly → §1.5.1 |

---

## 1.4 Edit Address Modal

**Trigger:** Per-entry ··· → Edit

Same fields as Add address modal, pre-filled with existing data. Button label changes from [Add] to [Save].

| Field | Example value |
|---|---|
| Country/region | United States [▼] |
| Name | lauda |
| Organization | MS |
| Street address | [existing] |
| City | [existing] |
| State | [existing] |
| ZIP code | [existing] |
| Phone | [existing] |
| Email | [existing] |

**Actions:** [Save] · [Cancel]

---

## 1.5 Delete Address

Two separate paths lead to deletion. Both share the same confirmation modal.

---

### 1.5.1 Via Per-Entry ··· → Delete

**Trigger:** Per-entry ··· → Delete

Goes directly to confirmation — no checkbox selection step.

**Step 1 — Confirmation modal:**
> *"Delete address?"*
> *"Selected addresses will be permanently deleted from your Microsoft Account."*

Actions: [Delete] · [Cancel] · [X]

**Step 2 — Success toast:**
- ✓ **Address deleted.** [X]
- Page returns to updated list (or empty state if last address removed)

---

### 1.5.2 Via Section Header 🗑 (Bulk Delete)

**Trigger:** Click **🗑** trash icon in the Addresses section header

**Step 1 — Selection mode entered:**
- Header changes to: **Addresses** · *0 selected* · [Cancel] · [Delete *(greyed)*]
- Each entry shows ○ selection circle

**Step 2 — Select addresses:**
- Click circle → ✓ filled checkmark; counter updates: *N selected*
- [Delete] activates (black) once ≥ 1 selected

**Step 3 — Confirmation modal:**
> *"Delete address?"*
> *"Selected addresses will be permanently deleted from your Microsoft Account."*

Actions: [Delete] · [Cancel] · [X]

**Step 4 — Success toast:**
- ✓ **Address deleted.** [X]
- Page returns to updated list (or empty state if all removed)

---

*Source: WCP Browser Settings screenshots — folder `3c_Addresses_and_more`*
*Documented: 2026-04-22*
