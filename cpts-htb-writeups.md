# CPTS Prep — HTB Machine Writeups

[![Playlist](https://img.shields.io/badge/Playlist-Unofficial_CPTS_Prep-ff0000?logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLidcsTyj9JXItWpbRtTg6aDEj10_F17x5)
[![Writeups repo](https://img.shields.io/badge/writeups_repo-cpts--htb--writeups-blue?logo=github)](https://github.com/MonkeyDLuffy13/cpts-htb-writeups)
![Progress](https://img.shields.io/badge/Solved_myself-0%2F22-red)

Hands-on prep track for the **HTB Certified Penetration Testing Specialist (CPTS)** exam,
built on the [Unofficial CPTS Prep](https://www.youtube.com/playlist?list=PLidcsTyj9JXItWpbRtTg6aDEj10_F17x5)
playlist — 22 Hack The Box machines with full walkthroughs by [IppSec](https://www.youtube.com/@ippsec).

📚 **Full write-ups live in [cpts-htb-writeups](https://github.com/MonkeyDLuffy13/cpts-htb-writeups)** —
every machine documented recon → foothold → privesc, with report-style impact & remediation.

The checkboxes below track **my own solves**: solve the box myself → check the box →
then watch IppSec's walkthrough to catch what I missed.

---

## Track 1 — Active Directory core *(the heart of the CPTS exam)*

- [ ] [Forest](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/forest) — Windows AD · AS-REP Roasting → WinRM → DCSync
- [ ] [Active](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/active) — Windows AD · GPP cpassword → Kerberoasting → DCSync
- [ ] [Blackfield](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/blackfield) — Windows AD · AS-REP → BloodHound → LSASS dump → SeBackupPrivilege
- [ ] [Manager](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/manager) — Windows AD · MSSQL recon → password spray → AD CS ESC7
- [ ] [Administrator](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/administrator) — Windows AD · assume-breach ACL chain → DCSync
- [ ] [Outdated](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/outdated) — Windows AD · Follina phishing → shadow credentials → WSUS abuse
- [ ] [Vintage](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/vintage) — Windows AD · machine password → gMSA → targeted Kerberoast → RBCD

## Track 2 — Windows foothold & privilege escalation

- [ ] [Remote](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/remote) — Windows · NFS leak → Umbraco RCE → TeamViewer decrypt
- [ ] [Access](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/access) — Windows · FTP mdb leak → PST mail → runas /savecred
- [ ] [Driver](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/driver) — Windows · printer panel → .scf NTLM leak → driver hijack
- [ ] [Sekhmet](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/sekhmet) — Windows · node-serialize RCE → sssd abuse → LDAP injection → DPAPI
- [ ] [Hospital](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/hospital) — Windows · .phar upload → kernel privesc → Ghostscript phishing

## Track 3 — Linux & web exploitation

- [ ] [Soccer](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/soccer) — Linux · Tiny File Manager → WebSocket SQLi → doas dstat
- [ ] [Delivery](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/delivery) — Linux · helpdesk mail enum → Mattermost → config reuse
- [ ] [MetaTwo](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/metatwo) — Linux · BookingPress SQLi → WordPress XXE → vault crack
- [ ] [Shoppy](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/shoppy) — Linux · NoSQL injection → credential reuse → docker group
- [ ] [Agile](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/agile) — Linux · path traversal → Werkzeug PIN → session theft
- [ ] [Trick](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/trick) — Linux · SQLi + LFI → mail poisoning → fail2ban hijack

### UHC event boxes

- [ ] [Union](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/uhc-union) — Linux · SQLi → X-Forwarded-For command injection
- [ ] [Pressed](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/uhc-pressed) — Linux · wp-config leak → XML-RPC abuse → PwnKit
- [ ] [LogForge](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/uhc-logforge) — Linux · Log4Shell ×2 → Tomcat path confusion

## Track 4 — Insane: containers & pivoting

- [ ] [Reddish](https://github.com/MonkeyDLuffy13/cpts-htb-writeups/tree/main/writeups/reddish) — Linux · Node-RED RCE → Redis pivot → rsync injection → container escape

---

## Exam skill map

| CPTS exam skill | Practice on |
|---|---|
| External reconnaissance & enumeration | every box — always go deeper than the nmap summary |
| Web application attacks | Soccer · MetaTwo · Shoppy · Agile · Pressed · Delivery |
| Password attacks & cracking | Forest · Active · Blackfield · Manager · Shoppy |
| AD exploitation & lateral movement | Track 1 — Forest → Vintage, in order |
| Windows privilege escalation | Driver · Access · Hospital · Sekhmet |
| Post-exploitation & pivoting | Reddish |

## Write-up conventions

Same rules as the rest of this profile:

- Every write-up is **reproducible step by step** — commands, request/response
  snippets, and the reasoning at each decision point, not just the happy path.
- Closes with an **impact + remediation** section, report-style.
- Tools that cost money are avoided where a free equivalent exists.

> ⚠️ All work is done on **intentionally vulnerable lab environments** (HTB) for
> educational purposes only.
