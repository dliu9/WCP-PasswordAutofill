# WCP Browser Settings — Passwords and Autofill

> **Path:** Settings → Passwords and autofill

This document covers all sub-sections under **Passwords and autofill**:
- [3A. Microsoft Password Manager](#3a-microsoft-password-manager)
- [3B. Payment Methods](#3b-payment-methods)

---

# 3A. Microsoft Password Manager

> **Path:** Passwords and autofill → Microsoft Password Manager

---

## Tree Structure

```
Passwords and autofill
└── Microsoft Password Manager
    ├── [Toggle] Ask to save passwords (OFF)
    ├── More settings →
    │   ├── [Toggle] Ask to save passwords (OFF)
    │   ├── [Toggle] Autofill passwords (ON)
    │   │   ├── ◉ Fill website password and sign in automatically.
    │   │   └── ○ Prompt for the device sign-in options before viewing or filling website password.
    │   ├── [Toggle] Scan passwords for leaks (OFF)
    │   ├── [Toggle] Show 'Reveal password' button (ON)
    │   └── [Toggle] Suggest strong passwords (OFF)
    └── Passwords [section]
        ├── 🔍 Search passwords
        ├── [+] Add password → Add password modal
        ├── [...] More options
        │   ├── Import passwords → Import flow (3 steps)
        │   └── Export passwords → Export flow (2 steps)
        ├── Password security check →
        │   ├── [Toggle] Enable leaked password scan in settings (OFF)
        │   └── Tabs: Leaked (0) | Reused (0) | Weak (n)
        │       └── [Weak] Create stronger passwords
        │           └── Per entry: [site] [password] [Change] [...]
        └── [Site entries] (grouped by site, e.g. google.com — 1 account)
            └── Site detail page →
                ├── Account name [copy]
                ├── Site URL [external link]
                ├── Password [eye] [copy]
                ├── Note
                ├── [Edit] → Edit password modal
                └── [Delete]
```

---

## 3A.1 Microsoft Password Manager — Main Page

**Path:** Passwords and autofill / Microsoft Password Manager

| Setting | State | Description |
|---|---|---|
| Ask to save passwords | OFF | Allow Copilot to ask to save your passwords and keep them safe. |

| Element | Description |
|---|---|
| More settings → | Opens the full settings sub-page (see §3A.1.1) |
| Passwords [section] | Lists all saved passwords with search, add, and more options |
| 🔍 Search passwords | Filter saved password entries |
| + Add | Opens Add password modal (see §3A.1.2) |
| ... | Opens Import / Export dropdown (see §3A.1.3) |
| Password security check → | Opens security check sub-page (see §3A.1.4) |
| [Site] — [n] account | Tap to open site password detail page (see §3A.1.5) |

---

## 3A.1.1 More Settings

**Path:** Passwords and autofill / Microsoft Password Manager / Settings

| Setting | State | Description |
|---|---|---|
| Ask to save passwords | OFF | Allow Copilot to ask to save your passwords and keep them safe. |
| Autofill passwords | ON | Allow Copilot to autofill existing passwords. |
| Scan passwords for leaks | OFF | Continuously scan your passwords in Copilot against known leaks and get notified. [Learn more] |
| Show 'Reveal password' button | ON | Shows a button to let you view your password as you type. This may not work on all sites. |
| Suggest strong passwords | OFF | Password suggestions work when Password Sync and Ask to save passwords are both set to on. |

### Autofill passwords — sub-options (shown when Autofill passwords is ON)

| Option | State | Description |
|---|---|---|
| ◉ Fill website password and sign in automatically. | Selected | Your saved passwords get auto-filled in web forms. Also, you can automatically sign-in to websites where this functionality exists. |
| ○ Prompt for the device sign-in options before viewing or filling website password. | Not selected | [Learn more] |

---

## 3A.1.2 Add Password Modal

**Trigger:** Click **+** button in the Passwords section header

| Field | Required | Placeholder |
|---|---|---|
| Website URL | ✱ | Enter Web URL |
| Username | ✱ | Enter username |
| Password | ✱ | Enter password (eye icon to reveal) |
| Note | Optional | Add notes |

> *"Adding the password here saves it only in Microsoft Edge. Make sure the password you save here matches your password for the website."*

**Actions:** [Cancel] [Add]

---

## 3A.1.3 More Options Menu (...)

**Trigger:** Click **...** button in the Passwords section header

| Option | State |
|---|---|
| → Import passwords | Active |
| \|→ Export passwords | Greyed out (when no passwords saved) |

---

### 3A.1.3.1 Import Passwords — 3-Step Flow

#### Step 1: Import passwords dialog

> *"To import passwords to your Copilot Account, from other application or select a CSV file."*

| Element | Value |
|---|---|
| Import from (dropdown) | Passwords CSV file |
| Help link | "Learn how to export a passwords CSV file from a password manager" |
| Primary action | [Choose CSV file] |
| Secondary action | [Cancel] |

#### Step 2: File picker dialog

| Element | Value |
|---|---|
| Window title | Import Passwords To Copilot |
| File type filter | Microsoft Excel Comma Separated Values |
| Actions | [Open] [Cancel] |

#### Step 3: Import success notice

> *"[n] passwords imported successfully!"*
> *"For your security, we recommend deleting your password file now. Once deleted, it cannot be recovered by anyone."*

| Element | Description |
|---|---|
| ☐ Checkbox | "Delete [filename].csv from your device." |
| [OK] | Closes the notice and returns to password list |

---

### 3A.1.3.2 Export Passwords — 2-Step Flow

#### Step 1: Export passwords dialog

> *"Your passwords will be visible to anyone who can see the exported file."*

| Action | Description |
|---|---|
| [Export] | Opens file save dialog |
| [Cancel] | Dismisses dialog |

#### Step 2: File save dialog

| Element | Value |
|---|---|
| Window title | Export Passwords From Copilot |
| Default file name | Microsoft Copilot Passwords.csv |
| Save as type | Microsoft Excel Comma Separated Values File (*.csv) |
| Actions | [Save] [Cancel] |

---

## 3A.1.4 Password Security Check

**Path:** Passwords and autofill / Microsoft Password Manager / Password security check

| Setting | State | Description |
|---|---|---|
| Enable leaked password scan in settings | OFF | Enable leaked password scan in settings |

### Tabs

| Tab | Count | Description |
|---|---|---|
| Leaked | 0 | Passwords found in known data breaches |
| Reused | 0 | Passwords used across multiple sites |
| Weak | (n) | Passwords that are easy to guess |

### Weak tab view

> *"Create stronger passwords"*
> *"Weak passwords are easier to guess. Keep your accounts more secure with..."*

Per entry displayed:

| Element | Description |
|---|---|
| Site domain | e.g. 1cm.hk.chinamobile.com |
| Username (if present) | Account name |
| •••••• [eye icon] | Masked password with reveal option |
| [Change] | Opens site in browser to change password |
| [...] | More options |

---

## 3A.1.5 Site Password Detail Page

**Path:** Passwords and autofill / Microsoft Password Manager / [site name]

### Single account view

| Field | Description | Actions |
|---|---|---|
| Account name | Username or email | [copy] |
| Site | Full URL | [external link] |
| Password | •••••••• | [eye icon] [copy] |
| Note | "No note added" or custom text | — |

**Actions:** [Edit] [Delete]

### Multiple accounts view (same site)

All accounts are shown expanded on the same page. Each entry shows:
- Account name [copy]
- Password •••••••• [eye icon] [copy]
- Site URL [external link]
- Note
- [Edit] [Delete]

---

## 3A.1.5.1 Edit Password Modal

**Trigger:** Click **[Edit]** on a site detail page

| Field | Required | Value |
|---|---|---|
| Site | Read-only | [URL — shown as clickable link] |
| Username | ✱ | [Enter username] |
| Password | ✱ | •••••• [eye icon] [copy] |
| Note | Optional | [Add notes] |

> *"Changing the password here updates it only in Microsoft Copilot. Make sure..."*

**Actions:** [Save] [Cancel]

---

*Source: WCP Browser Settings screenshots — folder `3a_Microsoft_Password_Manager`*
*Documented: 2026-04-22*

---
---

# 3B. Payment Methods

> **Path:** Passwords and autofill → Payment methods

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

## 3B.1 Payment Methods — Main Page

**Path:** Passwords and autofill / Payment methods

| Setting | State | Description |
|---|---|---|
| Save and fill payment methods | ON | Fills in payment forms with your saved payment methods. |
| Save security codes | ON | When enabled, Microsoft Copilot will securely store your security code (CVV/CVC) on this device, allowing for faster and more convenient checkout by automatically filling it in during the payment process. |
| Allow sites to check if you have saved payment methods | ON | *(highlighted row — no additional description visible)* |

| Element | Description |
|---|---|
| Payment methods [section] | Lists all saved cards with [+] Add button |
| + | Opens Add payment method modal (see §3B.1.1) |
| [Card entry] | e.g. Visa logo · *Visa •••• 8317* · *11/29* · [···] |
| ··· | Opens context menu: Edit / Delete (see §3B.1.2) |
| [Click card row] | Opens Edit payment method modal directly — Edit = View (see §3B.1.3) |

---

## 3B.1.1 Add Payment Method Modal

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

## 3B.1.2 Card Entry — Context Menu (···)

**Trigger:** Click **···** on a saved card entry

| Option | Action |
|---|---|
| Edit | Opens Edit payment method modal → §3B.1.3 |
| Delete | Removes the saved card |

---

## 3B.1.3 Edit Payment Method Modal (= View Card)

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

---
---

# 3C. Addresses and More

> **Path:** Passwords and autofill → Addresses and more

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

## 3C.1 Addresses and More — Main Page

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
| [Add address] button | Same trigger as [+] — opens Add address modal (see §3C.1.1) |

### With saved addresses

| Element | Description |
|---|---|
| [+] | Opens Add address modal (see §3C.1.1) |
| [🗑] | Enters bulk selection/delete mode (see §3C.1.5.2) |
| [···] | Opens Import / Export section menu (see §3C.1.2) |
| Address entry | Person icon · **Name** · Summary line (phone, email, street…) · [···] |
| Per-entry [···] | Opens Edit / Delete context menu (see §3C.1.3) |

---

## 3C.1.1 Add Address Modal

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

## 3C.1.2 Section Header ··· Menu

**Trigger:** Click **···** in the Addresses section header

| Option | State | Notes |
|---|---|---|
| →\| Import addresses | Disabled | Feature not yet implemented |
| \|→ Export addresses | Active | Opens file save dialog → §3C.1.2.1 |

---

## 3C.1.2.1 Export Addresses — File Save Dialog

| Element | Value |
|---|---|
| Window title | Save As |
| Default file name | `Microsoft_Copilot_Forms_YYYY_MM_DD.json` *(date-stamped)* |
| Save as type | JSON File (*.json) |
| Actions | [Save] [Cancel] |

> **Note:** Export format is **JSON** — different from passwords (CSV).

---

## 3C.1.3 Per-Entry ··· Context Menu

**Trigger:** Click **···** on a saved address entry row

| Option | Action |
|---|---|
| ✏️ Edit | Opens Edit address modal → §3C.1.4 |
| 🗑 Delete | Opens Delete confirmation modal directly → §3C.1.5.1 |

---

## 3C.1.4 Edit Address Modal

**Trigger:** Per-entry ··· → Edit

Same fields as Add address modal, pre-filled with existing data. Button changes from [Add] to [Save].

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

## 3C.1.5 Delete Address

Two paths — both share the same confirmation modal.

### 3C.1.5.1 Via Per-Entry ··· → Delete

**Trigger:** Per-entry ··· → Delete — goes directly to confirmation, no selection step.

**Step 1 — Confirmation modal:**
> *"Delete address?"*
> *"Selected addresses will be permanently deleted from your Microsoft Account."*

Actions: [Delete] · [Cancel] · [X]

**Step 2 — Success toast:** ✓ **Address deleted.** [X] — list updates.

---

### 3C.1.5.2 Via Section Header 🗑 (Bulk Delete)

**Trigger:** Click **🗑** in the Addresses section header

**Step 1 — Selection mode:** Header → *Addresses · 0 selected* · [Cancel] · [Delete *(greyed)*]; each entry shows ○ circle

**Step 2 — Select:** Click circle → ✓; counter updates to *N selected*; [Delete] activates (black)

**Step 3 — Confirmation modal:**
> *"Delete address?"*
> *"Selected addresses will be permanently deleted from your Microsoft Account."*

Actions: [Delete] · [Cancel] · [X]

**Step 4 — Success toast:** ✓ **Address deleted.** [X] — list updates.

---

*Source: WCP Browser Settings screenshots — folder `3c_Addresses_and_more`*
*Documented: 2026-04-22*
