# 🛡️ Cyber Shield SOC • Enterprise Security Operations & Autonomous Threat Defense

[![Version](https://img.shields.io/badge/version-v6.0.0-00f2fe.svg)](https://github.com/)
[![License](https://img.shields.io/badge/license-MIT-10b981.svg)](https://opensource.org/licenses/MIT)
[![Security Standard](https://img.shields.io/badge/standard-NIST%20SP%20800--61%20%7C%20ISO%2027001-blue.svg)](https://csrc.nist.gov/)
[![Offline First](https://img.shields.io/badge/offline-100%25%20Supported-purple.svg)](https://github.com/)

**Cyber Shield SOC v6.0** is an enterprise Security Operations Center (SOC) and Autonomous Threat Defense platform. Built with an offline-first client architecture, it unifies device registration, autonomous threat mitigation, code forensics, and governance across 21 core security topics.

---

## 📑 Comprehensive Topic Directory (Every Topic in the System)

### Topic 1: Portal Gateway & Device Enrolment
* **Location:** `tab-landing`
* **Purpose:** Public landing gate serving device owners and administrators.
* **Capabilities:**
  * **3-Step Device Enrolment:** Captures Full Name, Phone, Email, Hardware Type (Smartphone, Laptop, Desktop, Tablet, Server), OS (iOS, Android, Windows, macOS, Linux), and Network.
  * **Instant 6-Digit OTP Dispatch:** Automated SMS/Email code verification with an unlimited task runtime.
  * **Endpoint Shield Attestation:** Generates a unique protection key (e.g., `CS50-7F89A`), configures MDM profiles, and activates 24/7 autonomous shield.
  * **My Device Self-Service Lookup:** Enter endpoint ID to verify real-time health, incident history, and 8-point security guidelines.

### Topic 2: Security Overview Dashboard
* **Location:** `tab-overview`
* **Purpose:** Real-time executive situational awareness and SLA compliance tracking.
* **Capabilities:**
  * **Overall Security Posture Score:** Real-time score (91/100 EXCELLENT) evaluated across 4 domains (Perimeter Gateway, Mobile Shield, Identity/UEBA, DLP).
  * **Response Performance SLAs:** Mean Time to Detect (MTTD: 1.2s) and Mean Time to Respond (MTTR: 4.8s).
  * **24-Hour Threat Trend Spline:** HTML5 Canvas line chart tracking hourly threat volume.
  * **Severity Distribution:** Live breakdown across Critical (4), High (7), Medium (2), and Low (2).

### Topic 3: Incidents Management & Case Tracking
* **Location:** `tab-incidents`
* **Purpose:** Formalized Computer Security Incident Response (CSIRT) case lifecycle.
* **Capabilities:**
  * **Incident Search:** Instant filtering across case ID, severity, title, analyst, and asset.
  * **Create Incident Modal:** Formalize new cases with severity levels, category, affected asset, and summary.
  * **Investigation Drawer:** Sliding drawer with timeline logs, threat summaries, and analyst observation notes.

### Topic 4: Security Alerts & Ingress Detections
* **Location:** `tab-alerts`
* **Purpose:** Triage raw ingress security detections and trigger autonomous quarantine.
* **Capabilities:**
  * Ingress alerts table displaying Alert ID, Severity, Threat Vector, Threat Attribution, Source IP, Affected Code Asset, and Confidence %.
  * Direct file task button to jump into code forensics.
  * Instant "Block" action to drop malicious traffic at the firewall.

### Topic 5: Live Topological Threat Map HUD
* **Location:** `tab-soc`
* **Purpose:** Real-time network topology visualizer with dynamic flow particles.
* **Capabilities:**
  * **Topological Canvas Mesh:** Visualizes data flows connecting External Ingress, Perimeter IPS, DMZ Gateway, IAM SSO, Customer DB, and Internal LAN.
  * **Flow Particles & Radar Pulses:** Normal traffic pulses green; malicious ingress pulses red and triggers perimeter shockwaves.
  * **Live Alert Feed:** Timestamped stream of active drops and mitigations.

### Topic 6: Threat Intelligence & IOC Management
* **Location:** `tab-threat-intel`
* **Purpose:** Curated STIX 2.1 Indicator of Compromise (IOC) registry.
* **Capabilities:**
  * Track threat scores (0–100), actor attributions (Cobalt Gang, Lazarus Group, Mirai, Scattered Spider, LockBit), and confidence levels.
  * Add IOC Modal for IPv4, Domain names, SHA-256 file hashes, and CVE identifiers.

### Topic 7: Cyber Attack Simulator Range
* **Location:** `tab-simulator`
* **Purpose:** Controlled attack simulation for stress-testing defensive pipelines.
* **Capabilities:**
  * **SYN Flood DDoS Attack:** High-volume TCP connection queue exhaustion simulation.
  * **Mobile Pegasus C2 Heartbeat:** Trojan cellular egress probe simulation.
  * **SQL Injection Probing:** Tautological database bypass probe simulation.

### Topic 8: Code Target Forensics & In-Memory Virtual Patching
* **Location:** `tab-source`
* **Purpose:** Zero-downtime hotfixing of vulnerable source code without service restart.
* **Capabilities:**
  * **Direct Task Switcher:** Toggle between `server.js (Line 42)`, `core/dlpEngine.js (Line 18)`, and `ml/anomaly.js (Line 89)`.
  * **Side-by-Side Diff:** Inspect vulnerable lines alongside in-memory kernel patch filters.
  * **Deploy Virtual Patch Button:** Instantly applies the fix in memory and updates the KPI ribbon.

### Topic 9: Phone & Mobile Endpoint Shield
* **Location:** `tab-mobile`
* **Purpose:** Comprehensive endpoint security for smartphones and tablets.
* **Capabilities:**
  * Live mobile device inventory (iPhone 15 Pro, Galaxy S24, Pixel 8) with active MDM agents.
  * **Android AFWall+ / iptables Generator:** Exportable hardened shell script (`.sh`) for rooted Android phones.
  * **Apple iOS Configuration Profile:** Exportable `.mobileconfig` payload profile.

### Topic 10: Protected Endpoints Directory
* **Location:** `tab-user-portal`
* **Purpose:** Enterprise directory of all registered workstations, laptops, and servers.
* **Capabilities:**
  * Track Device IDs, owner names, phone contacts, hardware specifications, OS versions, and network types.

### Topic 11: Admin Control Center & RBAC
* **Location:** `tab-admin-control`
* **Purpose:** Identity governance, session termination, and access control.
* **Capabilities:**
  * **Active Authenticated Sessions Table:** Monitor active tokens, IP addresses, and user-agents.
  * **Session Killswitch:** Terminate individual operator sessions or trigger a global session wipe.
  * **RBAC Permissions Matrix:** Configurable access permissions across Super Admin, Admin, SOC Operator, Security Auditor, and Registered User.

### Topic 12: Hardware & Ingestion Nodes Cluster
* **Location:** `tab-hardware-monitor`
* **Purpose:** Distributed telemetry ingestion nodes and hardware health.
* **Capabilities:**
  * Real-time status cards for `LOCAL-SOC-HOST`, `EDGE-GW-01`, `CORE-AUTH-NODE`, `STORAGE-DB-01`, and `SOC-HONEYPOT-01`.
  * Monitor CPU, RAM, Disk I/O, Operating Temperature, and Ingress throughput.

### Topic 13: 2FA & TOTP Verification Panel
* **Location:** `tab-verification-panel`
* **Purpose:** Two-factor identity attestation and emergency recovery.
* **Capabilities:**
  * **Live Rolling TOTP Authenticator:** Displays current 6-digit rolling code (`777888`).
  * **Emergency Scratch Codes:** Single-use cryptographic backup keys (`CS-BCK-A8F1-92D4`) with instant regeneration.

### Topic 14: Tamper-Evident SHA-256 Cryptographic Audit Ledger
* **Location:** `tab-audit-trail`
* **Purpose:** Immutable audit record for compliance and forensic admissibility.
* **Capabilities:**
  * Block records containing actor, role, action, target, and SHA-256 block hash.
  * **Verify Hash Chain:** Cryptographically verifies ledger block continuity.
  * **Export CSV:** One-click CSV export of the entire audit trail.

### Topic 15: Safe Database Diagnostic Console
* **Location:** `tab-database-schema`
* **Purpose:** Safe read-only SQL querying for forensic analysts.
* **Capabilities:**
  * Pre-loaded SQL diagnostic queries against `incidents`, `alerts`, `ioc_indicators`, and `users`.
  * Instant execution timer showing microsecond query latency.

### Topic 16: Security Panel & Quarantined Blacklist
* **Location:** `tab-security-panel`
* **Purpose:** Edge perimeter firewall and autonomous drop rules.
* **Capabilities:**
  * Quarantined Offender Blacklist with reason, timestamp, and autonomous block status.
  * Manual IP quarantine input and one-click unblock actions.

### Topic 17: Stealth Cloak & Decoys (Honeypots)
* **Location:** `tab-stealth`
* **Purpose:** Decoy services to tarpit, observe, and log unauthorized intruders.
* **Capabilities:**
  * Real-time feeds from `SSH-TARPIT-22`, `MYSQL-DECOY-3306`, and `/admin-portal` honeypots.
  * Captures intruder brute-force credentials and scanner fingerprints.

### Topic 18: Identity & UEBA Analytics
* **Location:** `tab-ueba`
* **Purpose:** User and Entity Behavior Analytics for anomaly detection.
* **Capabilities:**
  * ML-driven risk anomaly scoring.
  * Flagged anomalous off-hours logins, unauthorized proxy egress, and impossible travel patterns.

### Topic 19: Data Loss Prevention (DLP)
* **Location:** `tab-dlp`
* **Purpose:** Real-time egress inspection and PCI-DSS compliance.
* **Capabilities:**
  * Real-time packet sanitization using the Luhn algorithm to mask credit card numbers (`XXXX-XXXX-XXXX-1234`).
  * Enforces GDPR Art. 32 and HIPAA PII encryption rules.

### Topic 20: Enterprise Security Engine Settings
* **Location:** `tab-settings`
* **Purpose:** Fine-tune SOC automation sensitivity.
* **Capabilities:**
  * Configurable defense sensitivity (Aggressive, Balanced, Permissive).
  * Automated mobile firewall push mode toggles.
  * Offender IP quarantine duration controls (1 Hour, 24 Hours, Permanent).

### Topic 21: Compliance & Audit Reports Generator
* **Location:** `tab-reports`
* **Purpose:** Telemetry reporting aligned with international security frameworks.
* **Capabilities:**
  * Export structured compliance audit reports under **NIST SP 800-61 Rev. 2** and **ISO/IEC 27001**.
  * Downloadable JSON summary containing posture scores, incident tallies, and hash integrity seals.

---

## 📂 Project Directory Structure

```text
cyber-shield-soc/
├── index.html          # Main website page covering all 21 topics
├── style.css           # Complete responsive Cyberpunk/Enterprise CSS design system
├── script.js           # Consolidated JS controller, canvas visualizers, and offline mock engine
├── assets/             # Logos, icons, shield badges, and favicon
│   ├── favicon.svg     # SVG browser tab icon
│   ├── logo.svg        # Cyber Shield SOC brand emblem
│   └── shield-badge.svg# Autonomous defense active badge
├── README.md           # Complete documentation covering every topic
└── .gitignore          # Git exclusion rules for clean version control
```

---

## 🚀 Quickstart & Setup Guide

### Standalone Zero-Setup (Offline / Double-Click)
Double-click **`index.html`** in any browser. All interactive features, OTP verification, attack simulations, and localStorage persistence function directly with zero server dependencies.

### Local HTTP Server
```bash
# Using Python:
python -m http.server 8080

# Or using Node.js:
npx serve .
```

---

## 🔑 Default Credentials & Quick Test Keys

| Role | Username | Default Password |
| :--- | :--- | :--- |
| **Super Admin** | `SUNNY` | `MONKEY` *(or `AdminPass2026!`)* |
| **Security Admin** | `alex.rivera` | `AdminPass2026!` |

* **2FA Demo Code:** `777888`
* **Device OTP Code:** `742918` *(or the 6-digit number displayed on-screen)*
* **Pre-Enrolled Device IDs:** `CS50-DEV01`, `CS50-DEV02`, `CS50-DEV03`, `CS50-DEV04`
