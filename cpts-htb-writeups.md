# CPTS Prep — HTB Machine Writeups

[![Playlist](https://img.shields.io/badge/Playlist-Unofficial_CPTS_Prep-ff0000?logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLidcsTyj9JXItWpbRtTg6aDEj10_F17x5)
![Progress](https://img.shields.io/badge/Writeups-0%2F22-red)

Hands-on prep track for the **HTB Certified Penetration Testing Specialist (CPTS)** exam,
built on the [Unofficial CPTS Prep](https://www.youtube.com/playlist?list=PLidcsTyj9JXItWpbRtTg6aDEj10_F17x5)
playlist — 22 Hack The Box machines with full walkthroughs by [IppSec](https://www.youtube.com/@ippsec).

The playlist is curated around what the CPTS exam actually tests: **Active Directory
exploitation, privilege escalation, password attacks, and post-exploitation/pivoting** —
going well beyond the typical easy-box loop.

**How I use this tracker:** solve the box myself first → write the full write-up →
then watch IppSec's walkthrough to catch what I missed. Check the box only when the
write-up is done.

---

## Track 1 — Active Directory core *(the heart of the CPTS exam)*

- [ ] [Forest](https://www.youtube.com/watch?v=H9FcE_FMZio) — Windows AD · AS-REP Roasting → WinRM → DCSync
- [ ] [Active](https://www.youtube.com/watch?v=jUc1J31DNdw) — Windows AD · GPP cpassword → Kerberoasting → DCSync
- [ ] [Blackfield](https://www.youtube.com/watch?v=IfCysW0Od8w) — Windows AD · AS-REP → BloodHound path → LSASS dump
- [ ] [Manager](https://www.youtube.com/watch?v=lT2Tv0m4k7M) — Windows AD · MSSQL recon → password attacks → AD CS abuse
- [ ] [Administrator](https://www.youtube.com/watch?v=Miam4nw9pmE) — Windows AD · hard multi-step chain, end to end
- [ ] [Outdated](https://www.youtube.com/watch?v=TR132R1h3Ds) — Windows AD · patch-gap CVEs → domain compromise
- [ ] [Vintage](https://www.youtube.com/watch?v=-JM--KfVhpA) — Windows AD · certificate services abuse

## Track 2 — Windows foothold & privilege escalation

- [ ] [Remote](https://www.youtube.com/watch?v=iyYqgseKUPM) — Windows · service enumeration → password reuse
- [ ] [Access](https://www.youtube.com/watch?v=Rr6Oxrj2IjU) — Windows · MSSQL exploitation
- [ ] [Driver](https://www.youtube.com/watch?v=N2ahkarb-zI) — Windows · printer web panel → SeLoadDriverPrivilege abuse
- [ ] [Sekhmet](https://www.youtube.com/watch?v=vsgPsMZx59w) — Windows · ASP.NET exploitation
- [ ] [Hospital](https://www.youtube.com/watch?v=E8h0qWsBz6c) — Windows · web foothold → OpenFire privesc

## Track 3 — Linux & web exploitation

- [ ] [Soccer](https://www.youtube.com/watch?v=V_CkT7xyiCc) — Linux · WebSocket SQLi → WAF bypass → privesc
- [ ] [Delivery](https://www.youtube.com/watch?v=gbs43E71mFM) — Linux · app enumeration → credential reuse
- [ ] [MetaTwo](https://www.youtube.com/watch?v=Alx5KQWq7ZM) — Linux · WordPress plugin exploitation
- [ ] [Shoppy](https://www.youtube.com/watch?v=AJc53DUdt1M) — Linux · NoSQL injection → credential reuse
- [ ] [Agile](https://www.youtube.com/watch?v=ob-CwobmkKk) — Linux · password-manager app → credential theft
- [ ] [Trick](https://www.youtube.com/watch?v=ai98umjeO8M) — Linux · classic web exploitation chain

### UHC event boxes

- [ ] [Union](https://www.youtube.com/watch?v=z5pdizHDvt8) — Linux · event box
- [ ] [Pressed](https://www.youtube.com/watch?v=p8mIdm93mfw) — Linux · WordPress exploitation
- [ ] [LogForge](https://www.youtube.com/watch?v=XG14EstTgQ4) — Linux · log forging / auth bypass

## Track 4 — Insane: containers & pivoting

- [ ] [Reddish](https://www.youtube.com/watch?v=Yp4oxoQIBAM) — Linux · Redis RCE → container escape → multi-host pivoting

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
