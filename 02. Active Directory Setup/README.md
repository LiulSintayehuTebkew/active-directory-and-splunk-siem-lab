# 02 — Active Directory Setup

Set up a full Active Directory environment on Windows Server 2022. This covers everything from promoting the server to a domain controller, to creating the organizational structure and adding users.

---

## What was configured

**Forest and domain**
- Forest name: `Aksumite`
- Promoted Windows Server 2022 to Domain Controller
- Configured DNS on the DC

**Organizational Units**
- `HR` — contains one user account
- `IT` — contains one user account

**Domain join**
- Windows 10 target machine was joined to the Aksumite domain

---

## Screenshots

| File | What it shows |
|---|---|
| `01-domain-controller.png` | Server Manager confirming DC promotion |
| `02-my-forest-domain.png` | AD forest and domain structure |
| `03-IT-user.png` | IT OU with user account |
| `04-HR-user.png` | HR OU with user account |
| `05-joined-computer.png` | Windows 10 showing up in AD Computers |

---

## Why this matters

Active Directory is in almost every corporate Windows environment. Setting it up from scratch — forest, DC, OUs, users, domain join — covers the fundamentals that show up in both sysadmin and blue team roles. It also creates a realistic target for the attack simulation in folder 04.
