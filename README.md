# MonkeyDLuffy13

**Aspiring Application Security / Penetration Tester** — documenting every lab I solve, end to end.

I work across **web application security** and **mobile pentesting (Android & iOS)**:
solving hands-on labs, building small exploit tools and solver scripts, and
publishing step-by-step write-ups so anyone can reproduce the work.

---

## Repositories

| Repo | What's inside |
|---|---|
| [portswigger-labs-writeups](https://github.com/MonkeyDLuffy13/portswigger-labs-writeups) | **273 labs across 31 topics** of the PortSwigger Web Security Academy — full step-by-step solutions: SQLi, XSS, SSRF, JWT, GraphQL, request smuggling, prototype pollution, ... |
| [androgear](https://github.com/MonkeyDLuffy13/androgear) | **`gear` CLI** — Android pentesting toolkit for lab AND production APKs: one-command triage (framework/packer/tracker detection, obfuscation, signature schemes), deep-link & exported-component enumeration with ready `adb` triggers, secret hunting, a 12-hook Frida arsenal, pentest-report scaffolding |
| [cylab-academy-writeups](https://github.com/MonkeyDLuffy13/cylab-academy-writeups) | **100 writeups** for the CyLab Security Academy library (formerly picoCTF) — Web Exploitation, Reverse Engineering, Forensics, Crypto and Pwn, each closing with a report-ready impact/remediation paragraph |
| [android-pentesting-cheatsheet](https://github.com/MonkeyDLuffy13/android-pentesting-cheatsheet) | Android pentesting **from zero to hero** — 16 cheatsheets + scripts: lab setup, ADB, Frida/Objection, Burp MITM, IPC & deep links, native bypasses, MASVS checklist, automated MobSF triage pipeline |
| [ios-pentesting-cheatsheet](https://github.com/MonkeyDLuffy13/ios-pentesting-cheatsheet) | The iOS counterpart — 10 cheatsheets + a 7-script Frida pack + host tools: jailbreaks, IPA analysis, ObjC hooks, Keychain, pinning bypass, MASVS checklist |
| [8ksec-labs-writeups](https://github.com/MonkeyDLuffy13/8ksec-labs-writeups) | 8kSec Academy & Battlegrounds **Android & iOS exploitation labs** — 21 writeups (10 Android, 11 iOS) with PoC exploit apps and automated solver scripts |

## Find your way

| I'm interested in... | Start here |
|---|---|
| Web security (topic by topic) | [portswigger-labs-writeups](https://github.com/MonkeyDLuffy13/portswigger-labs-writeups) — pick a topic folder (sql-injection, ssrf, jwt, ...) |
| CTF challenges (picoCTF / CyLab) | [cylab-academy-writeups](https://github.com/MonkeyDLuffy13/cylab-academy-writeups) — indexed by category, difficulty, and a suggested learning order |
| Android pentesting, first steps | [android-pentesting-cheatsheet README](https://github.com/MonkeyDLuffy13/android-pentesting-cheatsheet) (roadmap + 60-second workflow) — or let [androgear triage](https://github.com/MonkeyDLuffy13/androgear) map an APK for you |
| Frida & dynamic analysis | [android file 06](https://github.com/MonkeyDLuffy13/android-pentesting-cheatsheet/blob/main/06-frida-objection.md) · [ios scripts/](https://github.com/MonkeyDLuffy13/ios-pentesting-cheatsheet/tree/main/scripts) |
| iOS pentesting | [ios-pentesting-cheatsheet cheatsheet/](https://github.com/MonkeyDLuffy13/ios-pentesting-cheatsheet/tree/main/cheatsheet) |
| Mobile Hacking Lab write-ups | [android writeups/](https://github.com/MonkeyDLuffy13/android-pentesting-cheatsheet/tree/main/writeups) · [ios writeups/](https://github.com/MonkeyDLuffy13/ios-pentesting-cheatsheet/tree/main/writeups) |

## Currently

- Working through the **Mobile Hacking Lab** track (51 labs, Android + iOS) — 23 write-ups so far
- Solving the **CyLab Security Academy** (picoCTF) challenge library and writing up every solve
- Growing a reusable **Frida bypass/script arsenal** for hardened apps
- Turning the MASVS checklist into repeatable per-app test runs

## Toolbox

![Burp Suite](https://img.shields.io/badge/Burp_Suite-Community-orange)
![Frida](https://img.shields.io/badge/Frida-dynamic_analysis-red)
![Objection](https://img.shields.io/badge/Objection-runtime_exploration-red)
![JADX](https://img.shields.io/badge/JADX-decompiler-blue)
![Ghidra](https://img.shields.io/badge/Ghidra-reverse_engineering-blue)
![MobSF](https://img.shields.io/badge/MobSF-automated_scanning-green)
![mitmproxy](https://img.shields.io/badge/mitmproxy-TLS_interception-green)
![adb](https://img.shields.io/badge/adb-Android-yellow)
![libimobiledevice](https://img.shields.io/badge/libimobiledevice-iOS-lightgrey)
![Python](https://img.shields.io/badge/Python-automation-informational)

## Notes

- All write-ups are for **educational purposes only**, on intentionally
  vulnerable lab environments and systems I am authorized to test.
- Everything is reproducible with **free tooling** — no paid licenses required.

---

[MIT licensed](https://github.com/MonkeyDLuffy13/android-pentesting-cheatsheet/blob/main/LICENSE) unless a repo says otherwise.
