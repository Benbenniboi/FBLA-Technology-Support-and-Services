# FBLA Technology Support & Services — Flashcards

**How to use:** Click any question to reveal the answer. Renders natively on **GitHub** (click to expand) and in **VS Code markdown preview** (works offline on the bus). Grouped by the 4 official test knowledge areas, weighted to their item counts, plus a rapid-fire cheat-sheet set and a role-play set.

**Where to spend bus time:** Hardware & Software Troubleshooting is the biggest bucket (30 items) — drill it hardest. Skim the cards tagged *[you likely know this]* fast. Give real attention to OSI, printers, Active Directory, load balancers, and service-desk terminology.

---

## IT Fundamentals (25 test items)

<details>
<summary>List the 7 OSI layers in order (bottom to top) and a mnemonic.</summary>

1 Physical, 2 Data Link, 3 Network, 4 Transport, 5 Session, 6 Presentation, 7 Application. Mnemonic (bottom→top): **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way.
</details>

<details>
<summary>Which OSI layer handles IP addresses and routers?</summary>

**Layer 3 — Network.** PDU = packet. Also handles routing and ICMP.
</details>

<details>
<summary>Which OSI layer handles MAC addresses and switches?</summary>

**Layer 2 — Data Link.** PDU = frame. Also Ethernet and ARP.
</details>

<details>
<summary>Which OSI layer handles ports, TCP, and UDP?</summary>

**Layer 4 — Transport.** PDU = segment. Handles reliability and flow control.
</details>

<details>
<summary>Which OSI layer handles encryption and compression?</summary>

**Layer 6 — Presentation.** (TLS/SSL, JPEG, ASCII — translation/formatting.)
</details>

<details>
<summary>Match the PDU to the layer: bit, frame, packet, segment.</summary>

Bit = Physical (L1), Frame = Data Link (L2), Packet = Network (L3), Segment = Transport (L4).
</details>

<details>
<summary>Which Windows features require Pro or higher (not Home)?</summary>

Domain join, BitLocker, Group Policy Editor (gpedit), and being an RDP host. Editions: Home, **Pro**, Enterprise, Education.
</details>

<details>
<summary>Name key macOS features (backup, search, encryption).</summary>

Time Machine (backup), Spotlight (search), FileVault (disk encryption), Finder, Mission Control, Keychain, Gatekeeper, Disk Utility. Installers: .dmg / .pkg / .app.
</details>

<details>
<summary>What does the Linux command fsck do?</summary>

**File System Check** — checks and repairs a Linux filesystem. It's the Linux equivalent of Windows' chkdsk.
</details>

<details>
<summary>ipconfig vs ifconfig — what and where?</summary>

Both view/manage IP config. **ipconfig** = Windows (`/all`, `/release`, `/renew`, `/flushdns`); **ifconfig** (or `ip`) = Linux.
</details>

<details>
<summary>What do ping, tracert, nslookup, and netstat do? [you likely know this]</summary>

ping = test reachability; tracert/traceroute = trace route hop-by-hop; nslookup = DNS queries; netstat = show active connections/ports.
</details>

<details>
<summary>32-bit vs 64-bit: key limits and compatibility?</summary>

32-bit (x86) addresses ~4 GB RAM max; 64-bit (x64) far more. A 64-bit OS runs most 32-bit apps; a 32-bit OS cannot run 64-bit apps.
</details>

<details>
<summary>CPU sockets: LGA vs PGA?</summary>

**LGA** = pins are on the motherboard/socket (chip has pads) — Intel style. **PGA** = pins are on the CPU chip — older AMD style.
</details>

<details>
<summary>Motherboard form factors, largest to smallest?</summary>

ATX > microATX > Mini-ITX.
</details>

<details>
<summary>Switch vs hub vs router?</summary>

**Hub** (L1) blindly broadcasts to all ports. **Switch** (L2) forwards by MAC address to the correct port. **Router** (L3) connects different networks and routes by IP.
</details>

<details>
<summary>Client vs server?</summary>

A **server** provides resources/services; a **client** requests and consumes them.
</details>

<details>
<summary>What does DNS do, what port, and key record types?</summary>

Resolves names (example.com) to IP addresses. **Port 53.** Records: A (IPv4), AAAA (IPv6), MX (mail), CNAME (alias), TXT (SPF/DKIM/verify), PTR (reverse).
</details>

<details>
<summary>What does DHCP do, what ports, and what happens if it fails?</summary>

Automatically assigns IP, subnet mask, gateway, and DNS to clients. **Ports 67/68.** Process = DORA (Discover, Offer, Request, Acknowledge). Failure → client gets **APIPA 169.254.x.x**.
</details>

<details>
<summary>Name the three private IPv4 ranges. [you likely know this]</summary>

10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16.
</details>

<details>
<summary>What is the loopback address?</summary>

127.0.0.1 (IPv4) / ::1 (IPv6) — tests the local TCP/IP stack.
</details>

<details>
<summary>How does information move across a network?</summary>

Data is split into **packets**; a **client** sends a **request**; a **server** responds. DNS resolves names to IPs; routers forward packets between networks.
</details>

<details>
<summary>What is SQL injection?</summary>

An attack that inserts malicious SQL through unsanitized input fields to read, alter, or destroy database data. Defense: input validation / parameterized queries.
</details>

<details>
<summary>What is a DDoS attack?</summary>

Distributed Denial of Service — many compromised machines flood a target with traffic to exhaust resources and deny legitimate access.
</details>

<details>
<summary>Name core digital security & privacy best practices.</summary>

VPN (encrypted tunnel), password manager (unique strong passwords), firewall (host + network), MFA/2FA, encryption, patching/updates, least privilege, anti-malware, 3-2-1 backups.
</details>

---

## Service Desk Operations (20 test items)

<details>
<summary>Help desk vs service desk?</summary>

**Help desk** = reactive, break/fix, single point of contact for incidents. **Service desk** = broader — also handles service requests and change, and aligns IT with business goals.
</details>

<details>
<summary>What is ITSM?</summary>

**IT Service Management** — designing, delivering, managing, and continually improving how IT services are provided. Focused on services and repeatable processes, not just fixing devices. ITIL is the common framework.
</details>

<details>
<summary>Describe the support tiers (0–3).</summary>

**Tier 0** = self-service (KB, FAQs, chatbots). **Tier 1** = first-line triage (resets, known fixes). **Tier 2** = deeper technical troubleshooting. **Tier 3** = experts/engineers/vendors.
</details>

<details>
<summary>When should a ticket be escalated?</summary>

When it exceeds your tier's skills, scope, or access — or when it risks breaching the **SLA**. Escalation can be **functional** (to a more skilled team) or **hierarchical** (to management).
</details>

<details>
<summary>What is the role of a ticketing system?</summary>

Creates a record for every issue to track status, priority, owner, and history; prevents lost requests; enables documentation, metrics, and a searchable knowledge base.
</details>

<details>
<summary>How is ticket priority typically determined?</summary>

**Impact × urgency** (how many are affected / how severe, versus how time-sensitive).
</details>

<details>
<summary>Name examples of service desk software.</summary>

JIRA and Zoho (also ServiceNow, Zendesk, Freshdesk). Functions: log/track/prioritize, assign/escalate, SLA tracking, knowledge base, reporting, automation.
</details>

<details>
<summary>What's the correct ORDER for removing malware? (high-yield)</summary>

1) Identify symptoms → 2) **Quarantine** the system → 3) Disable System Restore (Windows) → 4) Remediate (update definitions + scan/remove) → 5) Schedule scans and enable updates → 6) Re-enable System Restore / create a restore point → 7) Educate the user.
</details>

<details>
<summary>Common service-desk metrics?</summary>

MTTR (mean time to resolve), CSAT (customer satisfaction), FCR (first-contact resolution).
</details>

---

## Hardware & Software Troubleshooting (30 test items — the heaviest)

<details>
<summary>State the 6-step troubleshooting methodology (memorize).</summary>

1) Identify the problem (back up before changes). 2) Establish a theory of probable cause (question the obvious). 3) Test the theory. 4) Establish a plan of action and implement. 5) Verify full functionality + preventive measures. 6) Document findings, actions, outcomes.
</details>

<details>
<summary>How do you distinguish a hardware problem from a software problem?</summary>

Software issues live in the OS/apps (crashes, errors, malware) and often follow updates/installs. Hardware issues are physical and consistent across OSes (no power, beep codes, overheating, failing drive). Isolate using Safe Mode or a live USB.
</details>

<details>
<summary>Symptoms of a RAM problem?</summary>

Random BSODs/reboots, memory errors, failure to POST, app crashes. Fix: reseat, test (MemTest), verify matched pairs.
</details>

<details>
<summary>Symptoms of a CPU problem?</summary>

No boot, overheating/shutdowns under load, throttling. Check cooling, thermal paste, seating.
</details>

<details>
<summary>Symptoms of a failing storage drive?</summary>

Slow performance, **SMART errors**, clicking/grinding (HDD), corrupt/missing files, boot failures. Back up immediately; check cables; run chkdsk/fsck.
</details>

<details>
<summary>What is freeze spray used for in troubleshooting?</summary>

Rapidly cools a suspect component to reveal heat-related (thermal) faults. (Other tools: multimeter for voltage/continuity, compressed air for dust, PSU tester, cable tester.)
</details>

<details>
<summary>How do you decide to fix vs upgrade vs replace?</summary>

Weigh repair cost vs replacement, device age, parts availability, performance needs, and downtime. Upgrade (RAM/SSD) when cheap and life-extending; replace when repair nears replacement cost or the platform is obsolete.
</details>

<details>
<summary>Common Windows OS problems and first fixes?</summary>

BSOD, boot failures, "no OS found", slow performance, crashes. Fixes: Safe Mode, System Restore, Startup Repair/WinRE, `sfc /scannow`, `chkdsk`, MSConfig, Event Viewer, driver rollback.
</details>

<details>
<summary>Indicators of malware on a device?</summary>

Slowness, pop-ups, browser redirects, certificate warnings, new unknown programs, disabled security tools, encrypted/renamed files (ransomware), high CPU/disk/network use, altered hosts file.
</details>

<details>
<summary>Common quick hardware fixes ("off and on")?</summary>

Restart, full power-cycle (unplug + hold power to drain), **reseat** components/cables, check connections, update drivers/firmware, clear dust, let an overheating device rest.
</details>

<details>
<summary>USB connector types?</summary>

USB-A, USB-B, Mini-USB, Micro-USB, USB-C.
</details>

<details>
<summary>USB speeds: 2.0, 3.2 Gen 1, Gen 2, Gen 2x2, USB4?</summary>

2.0 = 480 Mbps; 3.2 Gen 1 (a.k.a. 3.0) = 5 Gbps; Gen 2 = 10 Gbps; Gen 2x2 = 20 Gbps; USB4 = 40 Gbps.
</details>

<details>
<summary>Common video connectors?</summary>

VGA (analog), DVI (A/D/I, single/dual link), HDMI, DisplayPort. Thunderbolt runs over USB-C.
</details>

<details>
<summary>RJ45 vs RJ11?</summary>

RJ45 = Ethernet (8 conductors). RJ11 = telephone (smaller).
</details>

<details>
<summary>Parts of an LCD?</summary>

LCD panel (liquid-crystal layer + polarizers), **backlight** (LED today; CCFL in older units), **inverter** (powers a CCFL backlight, DC→AC — common failure point), digitizer (touch layer), bezel. Wi-Fi antennas often run in the lid.
</details>

<details>
<summary>LCD panel types: TN vs IPS vs VA?</summary>

TN = fast, cheap, poor viewing angles. IPS = best color/angles. VA = high contrast. (OLED is self-emissive — not LCD, no backlight.)
</details>

<details>
<summary>What is the boot process order?</summary>

Power on → **POST** → firmware (BIOS/UEFI) → find boot device per boot order → load bootloader → load OS.
</details>

<details>
<summary>What can you configure in BIOS/UEFI?</summary>

Boot order, enable/disable devices, Secure Boot, TPM, virtualization (VT-x/AMD-V), and BIOS passwords.
</details>

<details>
<summary>MBR vs GPT?</summary>

**MBR**: max 2 TB, 4 primary partitions. **GPT**: >2 TB, up to 128 partitions, requires UEFI.
</details>

<details>
<summary>RAID 0, 1, 5, 6, 10 — define each.</summary>

0 = striping (speed, **no** redundancy, min 2). 1 = mirroring (min 2). 5 = striping + parity (min 3, survives 1 loss). 6 = double parity (min 4, survives 2 losses). 10 = mirror + stripe (min 4).
</details>

<details>
<summary>What is the laser printer imaging process order?</summary>

Processing → Charging → Exposing → Developing → Transferring → Fusing → Cleaning.
</details>

<details>
<summary>Printer won't print / shows offline — what do you check?</summary>

Wrong/offline driver, network/IP issue, stuck print queue (restart the **Print Spooler** service), USB/port/cable, paper/toner, printer set offline.
</details>

<details>
<summary>Common inkjet print-quality issues?</summary>

Faded output (low ink), streaks/missing lines (clogged heads — run cleaning), misalignment (calibrate). For laser: smearing that rubs off = fuser; repeating marks = drum.
</details>

<details>
<summary>Common mobile device issues and fixes?</summary>

Battery drain/overheating, won't connect (BT/Wi-Fi/cellular), app crashes, slow, won't update. Fixes: force-stop/clear cache, update/reinstall, restart, reset network settings, factory reset (back up first).
</details>

<details>
<summary>What does Safe Mode let you do?</summary>

Boots Windows with minimal drivers/services to isolate software issues, remove malware, roll back drivers, or fix a bad startup item.
</details>

---

## IT Management & Administration (25 test items)

<details>
<summary>What is the purpose of change management?</summary>

A structured process to make IT changes safely with minimal disruption (request → assess → approve → implement → review). Reduces risk, prevents outages, keeps an audit trail.
</details>

<details>
<summary>What elements belong in a change request document?</summary>

Date/time of change, **rollout (implementation) plan**, **backout/rollback plan**, anticipated impact and risk, scope, purpose, affected systems/users, approvals, and end-user acceptance.
</details>

<details>
<summary>What is a CAB?</summary>

**Change Advisory Board** — the group that reviews and approves proposed changes.
</details>

<details>
<summary>SSH — port and purpose?</summary>

**Port 22.** Secure, encrypted remote command-line access and file transfer (SFTP/SCP).
</details>

<details>
<summary>RDP — port and purpose?</summary>

**Port 3389.** Windows graphical Remote Desktop.
</details>

<details>
<summary>What is RMM?</summary>

**Remote Monitoring & Management** — tools used by IT teams/MSPs to monitor, patch, and manage many endpoints remotely at scale.
</details>

<details>
<summary>Name file transfer services/protocols. [you likely know this]</summary>

FTP/FTPS/SFTP (SFTP over SSH/22), TFTP, and cloud sync (Google Drive, OneDrive, Dropbox). Consider encryption, size limits, access control, versioning.
</details>

<details>
<summary>Key printer configuration settings?</summary>

Tray/paper-source (size/type), **duplex** (double-sided), **orientation** (portrait/landscape), collation, quality/DPI, color vs grayscale, default printer, sharing (local vs network).
</details>

<details>
<summary>Name the four printer types and one trait each.</summary>

Laser (toner + drum + fuser), Inkjet (liquid ink, needs head cleaning), Thermal (heat + special paper, receipts), 3D (additive — FDM filament or SLA resin).
</details>

<details>
<summary>What does a load balancer do?</summary>

Distributes incoming traffic across multiple servers to improve availability, scalability, performance, and redundancy. Methods: round-robin, least-connections. Hardware, software, or cloud (e.g., AWS ELB); uses health checks.
</details>

<details>
<summary>What is Active Directory?</summary>

Microsoft's directory service for Windows domains. Runs on a **domain controller**, is **LDAP**-based, uses **Kerberos** for authentication, and enables single sign-on.
</details>

<details>
<summary>What does Active Directory manage, and via what?</summary>

Objects: users, computers, groups, and **OUs** (organizational units). Centralized settings are pushed via **Group Policy (GPOs)**. Hierarchy: **forest → tree → domain**.
</details>

<details>
<summary>Define IaaS, PaaS, and SaaS.</summary>

**IaaS** = raw infrastructure (VMs/storage/networking) — e.g., AWS Lightsail. **PaaS** = platform/runtime to build & deploy apps. **SaaS** = finished software over the web — e.g., a hosted app like PhonoFlow.
</details>

<details>
<summary>Cloud deployment models and core characteristics?</summary>

Models: public, private, hybrid, community. Characteristics: on-demand self-service, rapid elasticity, measured/metered usage, scalability, high availability.
</details>

<details>
<summary>What is SPF? [you likely know this]</summary>

**Sender Policy Framework** — a DNS **TXT** record listing which servers/IPs may send mail for a domain; the receiver checks the sending IP against it.
</details>

<details>
<summary>What is DKIM? [you likely know this]</summary>

**DomainKeys Identified Mail** — adds a cryptographic signature to the message; the receiver verifies it using the public key published in DNS, proving integrity and authenticity.
</details>

<details>
<summary>What is DMARC, and what are its policy options?</summary>

**Domain-based Message Authentication, Reporting & Conformance** — a policy built on SPF + DKIM telling receivers what to do on failure: **none / quarantine / reject** — plus aggregate reports. Requires domain alignment.
</details>

---

## Rapid-Fire Cheat Sheet

<details>
<summary>Name the most-tested ports (number → protocol).</summary>

20/21 FTP · 22 SSH/SFTP · 23 Telnet · 25 SMTP · 53 DNS · 67/68 DHCP · 80 HTTP · 110 POP3 · 143 IMAP · 161/162 SNMP · 389 LDAP · 443 HTTPS · 445 SMB · 3389 RDP.
</details>

<details>
<summary>Reverse drill: SSH, RDP, HTTPS, SMB, DNS, DHCP — what ports?</summary>

SSH 22 · RDP 3389 · HTTPS 443 · SMB 445 · DNS 53 · DHCP 67/68.
</details>

<details>
<summary>Wi-Fi standards: a, b, g, n, ac, ax — bands and names?</summary>

a = 5 GHz; b/g = 2.4 GHz; n = Wi-Fi 4 (2.4/5); ac = Wi-Fi 5 (5 GHz); ax = Wi-Fi 6/6E (2.4/5/6 GHz).
</details>

<details>
<summary>File systems: NTFS, FAT32, exFAT, ext4, APFS — quick traits?</summary>

NTFS = Windows default (permissions, journaling). FAT32 = 4 GB file-size limit, very compatible. exFAT = large files + cross-platform (flash/SD). ext4 = Linux. APFS = macOS.
</details>

<details>
<summary>What is APIPA and what does it indicate?</summary>

169.254.x.x — a self-assigned address Windows gives when it **can't reach a DHCP server**. Seeing it = DHCP/connectivity problem.
</details>

---

## Role Play (the round that decides placement)

<details>
<summary>Which rubric category is worth the most, and how much?</summary>

**Conflict resolution & closure — 20 points** (double every other category). Top band requires: conflict resolved, situation closed, AND the judge/client is satisfied.
</details>

<details>
<summary>How is empathy scored?</summary>

As its own separate **10-point** category. This is a customer-service event — acknowledge frustration, be patient and diplomatic the entire time.
</details>

<details>
<summary>What earns the top band on "knowledge of terminology"?</summary>

Explaining terms clearly enough that the client could proceed on their own — i.e., translate to plain language, don't jargon-dump.
</details>

<details>
<summary>Role play timing structure?</summary>

20 minutes prep, 7-minute presentation (1-minute warnings on both). No separate Q&A, but judges may interrupt with questions mid-presentation. Going over time or breaking dress code = 5-point penalties.
</details>

<details>
<summary>What must every role play END with?</summary>

A close to a **satisfied client**: confirm the issue is resolved, summarize next steps, and explicitly ask if they're satisfied / need anything else — then thank them. Never trail off.
</details>

<details>
<summary>The 8-beat role-play framework?</summary>

1) Open + restate problem & impact. 2) Acknowledge the human (empathy). 3) State your approach. 4) Diagnose out loud with the 6-step method, defining terms simply. 5) Solution + implementation plan + resources (+ backup fix). 6) Prevention + document. 7) Close to a satisfied client (the 20-pointer). 8) Engage fully with judge interruptions.
</details>

---

*Good luck Monday, Ben. Drill troubleshooting hardest, lean on your PhonoFlow/home-lab strengths for the easy points, keep the role play warm with one walk-through, and sleep Sunday night.*
