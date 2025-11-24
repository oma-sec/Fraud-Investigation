## Overview
This document details the Open Source Intelligence (OSINT) techniques employed during the investigation of the JavaScript injection campaign. All methods utilized publicly available information and complied with ethical guidelines.

# 🕵️ OSINT Techniques for Cryptocurrency Threat Investigations

This document provides a technical overview of the OSINT methodologies used in the attribution and mapping of a cryptocurrency-related threat actor.  
The focus is on **professional, analyst-grade techniques**, with emphasis on identity correlation, infrastructure discovery, behavioral intelligence, and blockchain-based financial analysis.

---

# 1. Identity Intelligence (IDINT)

## 1.1 Alias & Handle Analysis
Threat actors commonly reuse signature behavioral patterns even when rotating usernames. Techniques applied:

### Handle Pivoting
- Cross-platform enumeration:
  - **Sherlock**
  - **Maigret**
  - **WhatsMyName**
  - NameChk OSINT indices
- Correlation methods:
  - String similarity metrics (Jaro–Winkler, Levenshtein)
  - Temporal alias reuse
  - Account creation chronology

### Linguistic Fingerprinting
Indicators:
- Repeated vocabulary and idioms  
- Characteristic punctuation  
- Frequent spelling anomalies  
- Cross-language writing patterns  

Tools:
- Stylometry heuristics  
- Metadata extraction from public posts  

---

# 2. Platform-Focused Intelligence

## 2.1 Telegram Intelligence (TGINT)
Public data only.

Collected:
- Channel/group metadata evolution  
- Admin/member changes  
- Active-hour analysis (timezone inference)  
- Media fingerprinting  

Tools:
- **Telethon** custom scripts  
- **tgstat**  
- TLSH / ssdeep hashing  

## 2.2 Underground Forum Enumeration
Data collected:
- Thread creation cadences  
- Burner-account lifespans  
- Reused crypto addresses in posts  
- Signature-link infrastructure reuse  
- Social engineering behavioral cues  

---

# 3. Technical OSINT (TECHOINT)

## 3.1 Passive Infrastructure Discovery

### Certificate Transparency Recon
Tools:
- **crt.sh**  
- **Censys**  
- Google CT Logs  

Use cases:
- Domain cluster correlation  
- Infrastructure reuse patterns  

### Passive DNS
Tools:
- **SecurityTrails**  
- **RiskIQ PassiveTotal**  
- **DNSDB Scout**

Applications:
- Host pairing  
- Infrastructure movement across ASNs  
- Historical DNS reconstruction  

### Passive Service Enumeration
Tools:
- **Shodan**  
- **Censys Search**

Indicators:
- JA3/JA4 fingerprints  
- Header personality consistency  
- Default banners from misconfigured servers  

---

# 4. Crypto-Financial OSINT (FININT)

## 4.1 Address Attribution
Techniques:
- Address reuse detection  
- Script signature comparison  
- Transaction graph depth analysis  
- Temporal correlation between spends  

Tools:
- **Breadcrumbs**  
- **Blockchair**  
- **Mempool.space**  
- **WalletExplorer**  

## 4.2 Behavioral Forensics on Public Ledgers
Heuristics:
- Mixer ingress/egress timing  
- Peel-chain identification  
- Change-address inference  
- Fee-rate fingerprinting  
- Multi-hop laundering patterns  

---

# 5. Content & Metadata Intelligence (METAINT)

## 5.1 Metadata Extraction
Tools:
- **ExifTool**  
- **mat2**  

Use cases:
- Detecting reposted media  
- Differential metadata comparison  
- Identifying editing devices or workflows  

## 5.2 Paste & Leak Monitoring
Platforms:
- Pastebin  
- Ghostbin  
- Rentry  
- Public leak mirrors  

Search patterns:
- Email fragments  
- Wallet addresses  
- C2 URLs  
- Unique linguistic indicators  

---

# 6. Behavioral OSINT (BEHAVINT)

## 6.1 Temporal Activity Profiling
Collected:
- Timezone estimation  
- Operational activity windows  
- High-risk action bursts  
- Message rhythm analysis  

## 6.2 Psychological & Communication Indicators
Indicators (non-medical):
- Risk tolerance  
- Improvisation vs. planning style  
- Escalation patterns  
- Tool preference stability  

---

# 7. Toolchain Summary

### Identity Correlation
- Sherlock  
- Maigret  
- WhatsMyName  
- Holehe  

### Infrastructure Intelligence
- Amass (passive)  
- Subfinder  
- TheHarvester  
- Shodan  
- Censys  

### Blockchain Intelligence
- Blockchair  
- Mempool.space  
- Breadcrumbs  
- BlockCypher  
- WalletExplorer  

### Automation & Custom Tools
- Custom Telethon scrapers  
- Python enrichment pipelines  
- Metadata batching utilities  
- Temporal correlation algorithms  

---

# 8. Investigation Workflow (OSINT-Only Perspective)

1. **Seed Collection**  
2. **Cross-Platform Enumeration**  
3. **Identity & Infra Correlation**  
4. **Public-Ledger Financial Mapping**  
5. **Analyst Review & Confidence Scoring**  
6. **Final Intelligence Packaging**  

---

# 9. Limitations of OSINT-Only Analysis

- No access to private APIs  
- Mixer interference  
- Spoofed infrastructure  
- Rapid actor migration  
- OSINT false-positive potential  

---

# 10. Analyst Best Practices

- Maintain strict OPSEC isolation  
- Avoid interacting with the threat actor  
- Require multi-indicator confirmation  
- Preserve reproducibility  
- Maintain full documentation trails  

---

These OSINT techniques reflect industry-grade practices applied specifically to cryptocurrency-enabled threat investigations.

