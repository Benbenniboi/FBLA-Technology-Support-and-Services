# FBLA Technology Support & Services — Nationals (NLC) Study Guide

**Built for:** Ben Scheibe | **Goal:** Place at NLC
**Aligned to:** The official 2025-2026 FBLA Competitive Event Guidelines (updated Nov 2025) — exact knowledge areas, item counts, and the official role-play rating sheet. Underlying technical reference: **CompTIA A+ 220-1101 (Core 1)** and **220-1102 (Core 2)**, plus Google IT Support / Coursera Technical Support Fundamentals and IBM's ITSM material.

> How to use this: The objective test is built from 4 fixed knowledge areas with set question counts (below). Study in proportion to those counts. Use Quizlet/BusyBear decks only for spaced-repetition drilling of facts (ports, OSI layers, RAID, commands). The substance you need is here.

---

## 1. Event Format (confirmed from the official guidelines)

Two phases, individual, Role Play category:

| | Details |
|---|---|
| **Objective test** | **100 questions, 50 minutes**, online, proctored, onsite at NLC. No reference materials. Devices off. Online calculator provided in-platform. You can **flag questions** for committee review. One piece of scratch paper provided. |
| **Role play** | **Top 15** objective-test scorers advance. **20 min prep**, **7 min presentation** (1-minute warnings for both). **No separate Q&A**, but **judges may interrupt with questions during the presentation.** |
| **Role-play materials** | FBLA gives you **2 notecards** (write on both sides, collected after) + pencil + the secret scenario. **No technology, reference materials, visuals, or props.** Presentations are **closed** to other attendees. |

**Eligibility / logistics worth knowing:**
- Each **state may submit up to 4 entries** per event.
- If you placed **top 10 in Help Desk** at a past NLC, you're **not eligible** for this event.
- **Photo ID** (physical or digital) must match your badge name.
- **Late arrival = 5-point penalty**; **dress-code violation = 5-point penalty.**
- Max **10 placements** recognized.
- **Don't discuss the role-play prompt** with anyone until the event concludes (confidentiality rule).

---

## 2. The Scoring Reality — where the event is actually won

**Phase 1 gets you in; Phase 2 wins it.** Only the **role-play score** determines final placement. Your objective test is used **only to break ties** in the final round (tiebreakers for *advancing* to top 15: 10 pre-selected questions → 20 pre-selected questions → fastest completion time).

**Inside the role play (100 points total), here's the exact point map. Study this like a playbook:**

| Scoring category | Max points | What "Exceeds" requires |
|---|---|---|
| **Conflict resolution & closure** | **20** ← double weight | Conflict resolved, situation closed, **AND the judge (client) is satisfied** |
| Understands role play & defines the problem(s) | 10 | Provides synopsis **AND** defines the problem(s), with expertise |
| Communicates a position on the scenario | 10 | States position on the problem **professionally** |
| Identifies a logical solution + implementation | 10 | Feasible solution **with an implementation plan and the resources** it needs |
| Empathy / diplomacy | 10 | Empathy + diplomacy that actively **add to the resolution** |
| Knowledge of terminology & components | 10 | Explains terms **clearly enough for the client to act on their own** (not jargon-dumping) |
| Statements well-organized & clearly stated | 10 | Logical sequence **and** well-organized |
| Confidence, body language, eye contact, voice projection | 10 | All four demonstrated |
| Effectively answers questions | 10 | **Interacts** with judges while fully answering |

**Three takeaways that should shape every practice rep:**
1. **The 20-pointer is closure with a satisfied client.** Always end by confirming the customer is happy and restating next steps. Never just trail off after proposing a fix.
2. **Empathy is graded separately and equally to your technical knowledge.** This is a *customer service* event. Acknowledge the user's frustration, be patient, be human.
3. **"Knowledge" scores highest when you translate, not when you flex.** The top band is explaining it so a non-technical client could proceed. Define your terms in plain language.

---

## 3. Your 7-Day Plan (mapped to the official knowledge areas)

Weight your time to the item counts: Troubleshooting (30) > IT Fundamentals (25) = IT Mgmt/Admin (25) > Service Desk (20).

- **Day 1 — Hardware & Software Troubleshooting, Part 1 (the 30-item area).** Methodology, HW vs SW, RAM/CPU/storage symptoms, common fixes, tools, cables/connectors, LCD parts, boot process.
- **Day 2 — Troubleshooting Part 2 + printers.** Printer issues + types, mobile device issues, Windows OS problems, malware indicators & removal, fix-vs-upgrade-vs-replace.
- **Day 3 — IT Fundamentals (25).** **OSI model**, Windows & macOS features, CLI (Windows + Linux incl. `fsck`), components, 32- vs 64-bit, networking basics, DNS/DHCP, IP, network hardware.
- **Day 4 — IT Fundamentals security + Service Desk Operations (20).** Security best practices & threats; help-desk importance, ITSM, escalation, tiers, ticketing, service desk software, malware ID/removal.
- **Day 5 — IT Management & Administration (25).** Change management, remote access (SSH/RMM/RDP/VPN), file transfer, printer config, load balancers, Active Directory, cloud (SaaS/PaaS/IaaS), DKIM/SPF/DMARC.
- **Day 6 — Role-play drills.** Run 4-5 timed mock scenarios (Section 8). Record yourself, score against the rubric, focus on closure + empathy.
- **Day 7 — Full review + light role-play polish.** Re-quiz weak areas, run the cheat sheet (Section 7), do 1-2 final timed reps. Sleep well.

**Daily:** 20-30 min flashcards — OSI layers, ports, RAID, malware-removal order, CLI commands, email-auth records.

---

# PART 1 — THE OBJECTIVE TEST (by official knowledge area)

---

## 1A. IT Fundamentals — 25 items

### The OSI Model (know all 7 layers, their PDUs, and example devices/protocols)
Mnemonic (bottom→top): **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way.

| # | Layer | PDU | Lives here |
|---|---|---|---|
| 7 | Application | Data | HTTP, FTP, SMTP, DNS, DHCP (user-facing protocols) |
| 6 | Presentation | Data | Encryption/decryption, compression, formatting (TLS/SSL, JPEG, ASCII) |
| 5 | Session | Data | Establishes/manages/ends sessions |
| 4 | Transport | Segment | **TCP/UDP, ports**, reliability, flow control |
| 3 | Network | Packet | **IP addressing, routers**, routing, ICMP |
| 2 | Data Link | Frame | **MAC addresses, switches**, Ethernet, ARP |
| 1 | Physical | Bit | Cables, hubs, NICs, signals, connectors |

Common test angles: which layer a router (3) vs switch (2) vs hub (1) operates at; where IP (3) vs MAC (2) vs ports (4) live; which layer does encryption (6).

### Operating systems
- **Windows (personal vs enterprise):** editions (Home, **Pro**, Enterprise, Education). Domain join, BitLocker, Group Policy, RDP host require **Pro+**. Enterprise/AD features for managed environments.
- **macOS (PC + mobile/iOS context):** Time Machine (backup), Spotlight (search), Finder, Mission Control, Keychain, FileVault (disk encryption), Gatekeeper, Disk Utility, .dmg/.pkg/.app.

### Command-line tools (Windows AND Linux — both are tested)
| Tool | Platform | Purpose |
|---|---|---|
| `ipconfig` | Windows | View/manage IP (`/all`, `/release`, `/renew`, `/flushdns`) |
| `ifconfig` / `ip` | Linux | View/manage IP |
| `ping` | Both | Test reachability |
| `tracert` (Win) / `traceroute` (Linux) | Both | Trace route to host |
| `nslookup` | Both | DNS queries |
| `netstat` | Both | Active connections/ports |
| **`fsck`** | **Linux** | **File System Check/repair (Linux equivalent of chkdsk)** |
| `chkdsk` | Windows | Check/repair disk |
| `sfc /scannow` | Windows | Repair system files |
| `chmod` / `chown` | Linux | Change permissions / ownership |
| `sudo` / `su` | Linux | Elevated privileges / switch user |
| `grep`, `cat`, `ls`, `cd`, `df`, `top`, `ps`, `kill` | Linux | File/process basics |

### Computer components
- **CPU** (cores/threads, clock, cache, socket — LGA pins-on-board vs PGA pins-on-chip), **motherboard** (form factors ATX > microATX > Mini-ITX; chipset; PCIe x1/x4/x8/x16; M.2 slots), **GPU** (integrated vs discrete, VRAM), RAM, storage, PSU, cooling (heatsink/fan, thermal paste, liquid).

### Software requirements: 32-bit vs 64-bit
- **32-bit (x86):** addresses max ~4 GB RAM. **64-bit (x64):** far more.
- A **64-bit OS runs most 32-bit apps**; a **32-bit OS cannot run 64-bit apps.**
- Check software needs against **CPU architecture, RAM, storage, and OS version.**

### Digital security & privacy best practices
VPN (encrypted tunnel for privacy/remote access), **password managers** (unique strong passwords), **firewalls** (host + network), MFA/2FA, encryption, patching/updates, least privilege, antivirus/anti-malware, secure backups (3-2-1).

### Common vulnerabilities & threats
Out-of-date/unpatched systems, **SQL injection** (malicious DB queries via unsanitized input), **DDoS** (flooding to deny service), XSS, phishing/social engineering, weak/default credentials, malware, zero-days, MITM/on-path, insider threats.

### How info moves across a network
Data is broken into **packets**; a **client** sends a **request**; a **server** responds. Protocols govern formatting/delivery; **DNS** resolves names→IPs; routers forward packets between networks.

### DNS and DHCP
- **DNS** = resolves human names (example.com) → IP addresses. Records: **A** (IPv4), **AAAA** (IPv6), **MX** (mail), **CNAME** (alias), **TXT** (SPF/DKIM/verify), **PTR** (reverse). Port **53**.
- **DHCP** = automatically assigns IP/subnet/gateway/DNS to clients (the DORA process: Discover, Offer, Request, Acknowledge). Ports **67/68**. Failure → **APIPA 169.254.x.x**.

### IP addressing
IPv4 (32-bit) vs IPv6 (128-bit). **Private ranges:** 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16. Public vs private + **NAT**. Static vs dynamic (DHCP). Loopback 127.0.0.1. Subnet mask (/24 = 255.255.255.0), default gateway, DNS server.

### Network hardware
**Switch** (L2, forwards by MAC to one port) vs **Hub** (L1, broadcasts to all) vs **Router** (L3, connects/route between networks by IP). Plus **modem** (ISP signal conversion), **access point** (Wi-Fi), **firewall**, **clients vs servers** (server provides resources/services; client requests them).

---

## 1B. Service Desk Operations — 20 items

### Why help/service desks matter
Single point of contact for IT issues; keep the business running (minimize downtime), improve productivity and user satisfaction, track/measure IT health, free up specialists. **Help desk** = reactive break/fix; **service desk** = broader (also handles requests, change, aligns IT to business).

### IT Service Management (ITSM)
The practice of designing, delivering, managing, and continually improving how IT services are provided to an organization — focused on **services and repeatable processes**, not just fixing devices. **ITIL** is the most common framework.

### Service desk software (named in objectives)
**JIRA** and **Zoho** (also ServiceNow, Zendesk, Freshdesk). Functions: log/track/prioritize tickets, assign and escalate, SLA tracking, knowledge base, reporting/analytics, automation.

### Ticketing systems
Create a record for every issue → **track status, priority, owner, and history**; ensure nothing is lost; enable documentation, metrics (MTTR, CSAT, first-contact resolution), and a searchable knowledge base. **Prioritization = impact × urgency.**

### Support tiers & escalation
- **Tier 0:** self-service (KB, FAQs, chatbots).
- **Tier 1:** first-line triage — password resets, known fixes.
- **Tier 2:** deeper technical troubleshooting.
- **Tier 3:** experts/engineers/vendors.
- **Escalate** when the issue **exceeds your tier's scope, skills, or access**, or when it risks breaching the **SLA**. Escalation can be **functional** (to a more skilled team) or **hierarchical** (to management).

### Problem-solving methodology
Use the formal 6-step method (see 1C). FBLA phrases it as: identify the problem → test theories → develop a plan of action.

### Malware identification & removal (best practices — order matters)
**Identify symptoms → quarantine the system → disable System Restore (Windows) → remediate (update definitions + scan/remove) → schedule scans and enable updates → re-enable System Restore / create a restore point → educate the end user.**

---

## 1C. Hardware & Software Troubleshooting — 30 items (the heaviest area)

### The 6-step troubleshooting methodology (memorize)
1. **Identify the problem** (gather info, question the user, note recent changes; **back up before changes**).
2. **Establish a theory of probable cause** (question the obvious; consider multiple causes).
3. **Test the theory.** Confirmed → proceed. Not confirmed → new theory or **escalate**.
4. **Establish a plan of action** and **implement** the solution.
5. **Verify full system functionality**; implement **preventive measures**.
6. **Document** findings, actions, and outcomes.

### Hardware vs software — how to tell
Software symptoms appear within the OS/apps (crashes, errors, slow apps, malware) and often follow updates/installs; hardware symptoms are physical/consistent across OSes (no power, beep codes, overheating, failing drive, dead pixels). Reproduce in **Safe Mode** or with a live USB to isolate.

### RAM / CPU / storage symptoms
- **RAM:** random BSODs/reboots, memory errors, fails to POST, app crashes → reseat/test (MemTest), check matched pairs.
- **CPU:** no boot, overheating/shutdowns under load, throttling → cooling, thermal paste, seating.
- **Storage:** slow performance, **SMART errors**, clicking/grinding (HDD), missing/corrupt files, boot failures → back up immediately, check cables, run `chkdsk`/`fsck`.

### Tools (named in objectives)
**Multimeter** (voltage/continuity), **power supply tester**, **freeze spray** (cool a component to spot heat-related faults), **compressed air** (dust removal), cable tester, loopback plug, toner probe, POST card, anti-static strap.

### Fix vs upgrade vs replace
Weigh **cost of repair vs replacement**, age, availability of parts, performance needs, and downtime. Upgrade (RAM/SSD) when it's cheap and extends useful life; replace when repair cost approaches replacement or the platform is obsolete.

### Common Windows OS problems
**BSOD**, boot failures / "no OS found", slow performance, frequent crashes, services not starting, profile errors. **Fixes:** Safe Mode, System Restore, Startup Repair / WinRE, `sfc /scannow`, `chkdsk`, MSConfig, Event Viewer, driver rollback, reset.

### Malware indicators
Slow performance, pop-ups, browser redirects, certificate warnings, new/unknown programs, disabled security tools, renamed/encrypted files (ransomware), high CPU/disk/network usage, altered hosts file, unexpected outbound traffic. (Removal = the order in 1B.)

### Common hardware fixes ("turn it off and on")
Restart, fully power-cycle (unplug/hold power to drain), **reseat** components and cables, check connections, update drivers/firmware, clear dust, let an overheating device rest/cool.

### Cables & connectors
- **USB:** A, B, Mini, Micro, **USB-C**. Speeds: 2.0 = 480 Mbps; 3.2 Gen1 = 5 Gbps; Gen2 = 10 Gbps; Gen2x2 = 20 Gbps; USB4 = 40 Gbps.
- **Lightning** (Apple), **Thunderbolt** (over USB-C).
- **Video:** VGA (analog), DVI (A/D/I, single/dual link), **HDMI**, **DisplayPort**.
- **Network:** Cat5e/6/6a (RJ45), coax (F-connector), fiber (SC/LC/ST). **RJ45** = Ethernet, **RJ11** = phone.
- **Storage:** SATA (data + 15-pin power), M.2 (NVMe vs SATA keying).

### LCD types & parts
- **Parts:** LCD panel (liquid-crystal layer + polarizers), **backlight** (LED today; **CCFL** in older units), **inverter** (powers a CCFL backlight — converts DC→AC; a common failure point in older laptops), **digitizer** (touch layer), bezel, Wi-Fi antennas often run through the lid.
- **Panel types:** **TN** (fast, cheap, poor angles), **IPS** (best color/angles), **VA** (high contrast). OLED = self-emissive (not LCD; no backlight).

### Boot process & configuration
**Power on → POST → firmware (BIOS/UEFI) → locate boot device per boot order → load bootloader → load OS.** In **BIOS/UEFI** you set **boot order**, enable/disable devices, **Secure Boot**, **TPM**, **virtualization (VT-x/AMD-V)**, and BIOS passwords. **MBR** (≤2 TB, 4 primary partitions) vs **GPT** (>2 TB, up to 128 partitions, requires UEFI).

### Printers (troubleshooting side)
- **Connectivity:** wrong/offline driver, network/IP issue, spooler stuck (restart Print Spooler service), USB/port.
- **Refillables / consumables:** low toner/ink (faded), clogged inkjet heads (run cleaning), drum issues (repeating marks), fuser issues (smearing that rubs off), paper jams (rollers/path).

---

## 1D. IT Management & Administration — 25 items

### Change management
A structured process to make IT changes safely with minimal disruption: request → assess → approve → implement → review. Reduces risk, prevents outages, keeps an audit trail. Approval often via a **Change Advisory Board (CAB)**.

### Change request document elements (named in objectives)
**Time/date of the change**, **rollout (implementation) plan**, **backout/rollback plan**, **anticipated impact and risk**, scope, purpose/reason, affected systems/users, approvals, and **end-user acceptance**.

### Remote access — methods & protocols
Used to troubleshoot, test, install, and update systems remotely.
- **SSH** (port 22) — secure encrypted CLI/remote.
- **RDP** (port 3389) — Windows graphical remote desktop.
- **VPN** — encrypted tunnel into a private network.
- **RMM (Remote Monitoring & Management)** — tools (used by IT teams/MSPs) to monitor, patch, and manage many endpoints at scale.
- Also: VNC (cross-platform GUI), Telnet (insecure — avoid).

### File transfer services & protocols
**FTP/FTPS/SFTP** (SFTP over SSH/22), TFTP, **cloud storage/sync** (Google Drive, OneDrive, Dropbox). Considerations: encryption in transit, file size limits, access control/sharing, versioning.

### Printer configuration settings
**Tray/paper-source settings** (size/type per tray), **duplex** (double-sided), **orientation** (portrait/landscape), collation, print quality/DPI, color vs grayscale, default printer, and **sharing** (local vs network/TCP-IP printing).

### Printer types
- **Laser** — toner + drum; imaging order: **Processing → Charging → Exposing → Developing → Transferring → Fusing → Cleaning.**
- **Inkjet** — liquid ink + print heads; needs head cleaning/calibration.
- **Thermal** — heat + special paper (receipts).
- **3D** — additive; FDM (filament) vs SLA (resin). *(You'll be strong here from the Bambu A1.)*

### Load balancers
Distribute incoming traffic across multiple servers to improve **availability, scalability, performance, and redundancy**. Methods: round-robin, least-connections, etc. Hardware appliance, software, or cloud (e.g., AWS ELB). Pair with health checks so traffic only goes to healthy servers.

### Active Directory (AD)
Microsoft's **directory service** for Windows domains. Runs on a **domain controller**; **LDAP**-based; uses **Kerberos** for authentication and enables **single sign-on**. Manages **objects** (users, computers, groups, **OUs**) and pushes centralized settings via **Group Policy (GPOs)**. Hierarchy: **forest → tree → domain.**

### Cloud service models
- **IaaS** — raw infrastructure (VMs, storage, networking); you manage OS up. *(AWS Lightsail = IaaS — your PhonoFlow host.)*
- **PaaS** — platform/runtime to build/deploy apps; provider manages the stack below.
- **SaaS** — finished software over the web. *(PhonoFlow itself is SaaS.)*
- Plus deployment models: public, private, hybrid, community; characteristics: on-demand self-service, elasticity, measured/metered usage, scalability, high availability.

### Spam mitigation — email authentication (you already know this from PhonoFlow)
- **SPF (Sender Policy Framework):** DNS **TXT** record listing which servers/IPs may send mail for the domain. Receiver checks the sending IP against it.
- **DKIM (DomainKeys Identified Mail):** adds a **cryptographic signature** to the message; receivers verify it with the **public key published in DNS** — proves integrity + authenticity.
- **DMARC (Domain-based Message Authentication, Reporting & Conformance):** a **policy** built on SPF + DKIM that tells receivers what to do on failure (**none / quarantine / reject**) and sends **aggregate reports**. Requires **alignment** between the From domain and the SPF/DKIM domain.

---

# PART 2 — ROLE PLAY: Engineered to the Official Rubric

You get a tech-support scenario (an end user or business with an IT problem). 20 min to prep with 2 notecards, then a 7-minute presentation to judges who **act as the client/manager and may interrupt with questions.**

## The framework (write this skeleton on Notecard 1 the moment prep starts)

Each step below is tagged to the rubric category it scores. Hit all of them.

1. **Open professionally + restate the problem** *(→ Understands & defines problem, 10 pts).* Introduce yourself and your role ("IT support specialist"). Restate the issue and its **business impact** ("So your team can't access email, which is blocking invoicing — did I get that right?"). This proves understanding and starts the empathy clock.
2. **Acknowledge the human** *(→ Empathy/diplomacy, 10 pts).* "I understand how disruptive this is, and I'll get it sorted." Stay patient and warm throughout — this is graded the entire time.
3. **State your position / approach** *(→ Communicates position, 10 pts).* Briefly say how you'll tackle it ("Let's identify the cause, then I'll walk you through the fix and how to prevent it.").
4. **Diagnose out loud with method** *(→ Knowledge of terminology, 10 pts).* Walk the **6-step methodology**: what info you'd gather, 2-3 plausible causes, how you'd test each. **Define every technical term in plain language** as you go — the top score is the client being able to follow along.
5. **Give a solution + implementation plan + resources** *(→ Logical solution & implementation, 10 pts).* Provide a clear primary fix **and a backup**, the **steps to implement**, and what's **needed** (tools, access, time, escalation to Tier 2/vendor if warranted). Name the ITSM mechanics where they fit (open a ticket, SLA, escalation).
6. **Prevent recurrence** *(→ strengthens solution + knowledge).* One preventive measure: patch, backup, MFA, user training, monitoring — and **document it** in the ticket/KB.
7. **Close to a satisfied client** *(→ Conflict resolution & closure, 20 pts — the big one).* Confirm the problem is resolved, **summarize next steps**, and **explicitly check the client is satisfied**: "Does that fully resolve it for you? Anything else I can help with?" Then thank them. **Do not end without this.**
8. **Handle interruptions as opportunities** *(→ Answers questions, 10 pts).* When a judge asks something, **engage** — answer fully and check it landed. Interaction (not just a correct answer) is the top band.

## Timing (7 minutes)
~1 min open + restate/empathy · ~2 min diagnose with method · ~2 min solution + implementation + prevention · ~1.5 min closure + satisfaction check · buffer for judge questions throughout. Practice with a timer until the shape is automatic. Watch for the 1-minute warning.

## Notecard strategy (you only get 2)
- **Card 1:** the 8-step framework skeleton above + the 6 troubleshooting steps + the malware-removal order.
- **Card 2:** scenario-specific notes — the stated problem, likely causes, your chosen fix, backup fix, prevention, and your closing line.

## Delivery (the two 10-pt delivery categories)
- **Organized & clear:** follow the framework so there's a visible logical sequence; don't ramble.
- **Confidence + body language + eye contact + voice projection:** all four are required for full marks. **Talk to the judges as the client**, glance at cards rather than reading, sit/stand with poise, project. Slow down — nerves speed you up.

## Pitfalls that cost points
- Trailing off without confirming satisfaction → forfeits much of the 20-pt closure category.
- Pure jargon with no plain-language translation → caps the knowledge category.
- Forgetting empathy because you're focused on the tech → loses a full 10-pt category.
- Going over 7 minutes or violating dress code → **5-point penalties.**
- Reading off the notecard the whole time → tanks the delivery categories.

---

# PART 3 — One-Page Cheat Sheet (print this)

**OSI (bottom→top, "Please Do Not Throw Sausage Pizza Away"):** 1 Physical (bits/hub) · 2 Data Link (frames/switch/MAC) · 3 Network (packets/router/IP) · 4 Transport (segments/TCP-UDP/ports) · 5 Session · 6 Presentation (encryption) · 7 Application (HTTP/DNS/SMTP)

**Ports:** 20/21 FTP · 22 SSH/SFTP · 23 Telnet · 25 SMTP · 53 DNS · 67/68 DHCP · 80 HTTP · 110 POP3 · 143 IMAP · 161/162 SNMP · 389 LDAP · 443 HTTPS · 445 SMB · 3389 RDP

**Troubleshooting (6 steps):** Identify → Theory → Test → Plan/Implement → Verify (+prevent) → Document

**Malware removal order:** Identify → Quarantine → Disable System Restore → Remediate (update+scan) → Schedule scans/updates → Re-enable System Restore → Educate user

**Support tiers:** 0 self-service · 1 first-line · 2 technical · 3 experts/vendor — escalate beyond your scope or to protect the SLA

**Change request doc:** date/time · rollout plan · backout/rollback plan · impact/risk · scope · approval (CAB) · user acceptance

**Email auth:** SPF (TXT = allowed senders) · DKIM (signature verified via DNS public key) · DMARC (policy none/quarantine/reject + reports)

**Cloud:** IaaS (infra — Lightsail) · PaaS (platform) · SaaS (software — PhonoFlow)

**Remote/transfer:** SSH 22 · RDP 3389 · VPN tunnel · RMM (manage many endpoints) · FTP/SFTP · Drive/OneDrive

**RAID:** 0 stripe (no redundancy) · 1 mirror · 5 stripe+parity (min 3) · 6 double parity (min 4) · 10 mirror+stripe (min 4)

**Private IPs:** 10/8 · 172.16/12 · 192.168/16 · APIPA 169.254.x.x (DHCP failed) · loopback 127.0.0.1

**Wi-Fi:** a=5GHz · b/g=2.4GHz · n=Wi-Fi 4 · ac=Wi-Fi 5 · ax=Wi-Fi 6/6E

**Partitions:** MBR ≤2TB/4 primary · GPT >2TB/128 parts (UEFI)

**File systems:** NTFS (Win) · FAT32 (4GB file limit) · exFAT (big files, cross-platform) · ext4 (Linux) · APFS (macOS)

**Laser print order:** Processing → Charging → Exposing → Developing → Transferring → Fusing → Cleaning

**USB speeds:** 2.0=480M · 3.2 Gen1=5G · Gen2=10G · Gen2x2=20G · USB4=40G

**LCD parts:** panel · backlight (LED/CCFL) · inverter (CCFL only) · digitizer (touch)

**Linux CLI:** `fsck` (disk check) · `chmod`/`chown` · `sudo` · `grep` · `ifconfig`/`ip` · `ps`/`top`/`kill`

**AD:** domain controller · LDAP + Kerberos · users/computers/groups/OUs · Group Policy · forest→tree→domain

---

## Final Notes
- **Proportion your studying to the item counts:** Troubleshooting (30) is the biggest single bucket; don't shortchange it.
- **Two of your strengths are gift points:** DKIM/SPF/DMARC and cloud models (IaaS/SaaS) map straight onto your PhonoFlow work; the Linux CLI and networking objectives onto your home-lab/Debian work. Lock those down fast and spend saved time on OSI, printers, and the role play.
- **The role play is where placement happens — rehearse it out loud, on a timer, with someone interrupting you.** Optimize for the **20-point closure-with-a-satisfied-client** category and the separate **10-point empathy** category; most competitors under-invest in both.
- Sample test items and sample role plays are posted in **FBLA CONNECT** — pull those to calibrate to the real question style and practice with authentic prompts.
- Night before: light review, good sleep.

Go get it, Ben.
