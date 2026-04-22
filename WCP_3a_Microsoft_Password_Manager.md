# WCP Browser Settings — Passwords and Autofill / Microsoft Password Manager

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

## 1. Microsoft Password Manager — Main Page

**Path:** Passwords and autofill / Microsoft Password Manager

| Setting | State | Description |
|---|---|---|
| Ask to save passwords | OFF | Allow Copilot to ask to save your passwords and keep them safe. |

| Element | Description |
|---|---|
| More settings → | Opens the full settings sub-page (see §1.1) |
| Passwords [section] | Lists all saved passwords with search, add, and more options |
| 🔍 Search passwords | Filter saved password entries |
| + Add | Opens Add password modal (see §1.2) |
| ... | Opens Import / Export dropdown (see §1.3) |
| Password security check → | Opens security check sub-page (see §1.4) |
| [Site] — [n] account | Tap to open site password detail page (see §1.5) |

---

## 1.1 More Settings

**Path:** Passwords and autofill / Microsoft Password Manager / Settings

| Setting | State | Description |
|---|---|---|
| Ask to save passwords | OFF | Allow Copilot to ask to save your passwords and keep them safe. |
| Autofill passwords | ON | Allow Copilot to autofill existing passwords. |
| Scan passwords for leaks | OFF | Continuously scan your passwords in Copilot against known leaks and get notified. [Learn more] |
| Show 'Reveal password' button | ON | Shows a button to let you view your password as you type. This may not work on all sites. |
| Suggest strong passwords | OFF | Password suggestions work when Password Sync and Ask to save passwords are both set to on. |

### Autofill passwords — sub-options (shown when Autofill passwords is ON)

| Option                                                                              | State        | Description                                                                                                                         |
| ----------------------------------------------------------------------------------- | ------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| ◉ Fill website password and sign in automatically.                                  | Selected     | Your saved passwords get auto-filled in web forms. Also, you can automatically sign-in to websites where this functionality exists. |
| ○ Prompt for the device sign-in options before viewing or filling website password. | Not selected | [Learn more]                                                                                                                        |

---

## 1.2 Add Password Modal

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

## 1.3 More Options Menu (...)

**Trigger:** Click **...** button in the Passwords section header

| Option | State |
|---|---|
| → Import passwords | Active |
| \|→ Export passwords | Greyed out (when no passwords saved) |

---

### 1.3.1 Import Passwords — 3-Step Flow

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

### 1.3.2 Export Passwords — 2-Step Flow

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

## 1.4 Password Security Check

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

## 1.5 Site Password Detail Page

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

## 1.5.1 Edit Password Modal

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
