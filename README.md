# ⚠️ CONFIDENTIALITY NOTICE

For security reasons and in compliance with confidentiality agreements, sensitive information — including specific company names, real malicious code, and Indicators of Compromise (IOCs) — has been intentionally omitted from this case study.

However, I am authorized to discuss technical and methodological details in controlled environments under the protection of a Non-Disclosure Agreement (NDA).

---
[Summary](docs/summary.md)
---

## 📧 VERIFICATION & CONTACT

Given the significant impact of this case in the crypto ecosystem, legitimate organizations, technical recruiters, or security teams may request:

- Additional technical information  
- Identity verification and research authenticity  
- Details about the methodology applied  

The study was conducted anonymously via the Tor network to ensure the integrity and security of the investigation.

**Contact for legitimate verification:**  
`blusterc@proton.me`

---

## 🔍 NOTE ON ATTRIBUTION

This report describes the infrastructure, technical behavior, and tactics associated with the operator known by the alias **"***ed*"** in crypto fraud communities.

All conclusions are based on:

- Traffic analysis  
- Artifact correlation  
- On-chain tracking  
- Open-source investigation (OSINT)  

No statement in this document should be interpreted as a direct legal accusation against any specific individual. Attribution refers exclusively to the alias and the observed operations, following threat intelligence standards.

---

## ⚖️ POTENTIAL LEGAL FRAMING

The activities documented in this study include patterns that fall under:

- Crypto mixing  
- Electronic fraud  
- Malicious code injection  
- Malware distribution  
- Criminal association  
- Social engineering for criminal purposes  
- Money laundering  
- Use of false identity  

This study is intended solely for research, awareness, and security development purposes. Any legal action must be carried out by competent authorities.

---
Tracked Wallet Software with ["On-Chain" Analysis](docs/On-chain.md)

    Cake Wallet
    Wasabi Wallet
    JoinMarket
    Redacted: “Bl*** Py***mid” wallet/service and Illegal Mixer

---

### Message to the alias operator (ignore)

If the operator known as "*ed**" of the mentioned alias has accessed this report via URL mining or mention monitoring:

**ed**, as previously discussed, the technical and human recommendation is simple:  
Cease your activities and surrender to the competent authorities.

Your infrastructure, mixing patterns, and on-chain flows have been mapped. Continuing these operations only increases your legal and operational exposure. Stealing from innocent people is not a way to succeed in life.

---

# 🛡️ Ethics & Safety

- No PII is stored here  
- No complete malicious domains are included  (the both)
- No executable malicious code is present  
- All content follows Responsible Disclosure guidelines
🔍 Cryptocurrency JavaScript Injection Campaign Investigation

📖 Overview

A 5-month threat intelligence investigation into sophisticated social engineering campaigns distributing malicious JavaScript to cryptocurrency users, leading to transaction hijacking and credential theft across multiple exchanges.

Threat Type: Social Engineering + JavaScript Injection Attack
Distribution: Spam campaigns with significant reach (Million)
Social Engineering Lure: Fake profit promises and "easy money" claims
Specific Instruction: Attackers instruct victim to bypass security
Impact: Full session compromise, transaction interception, fund theft potential

🔧 Technical Investigation
Malware Analysis

The campaign utilized sophisticated multi-stage payloads with hexadecimal obfuscation and dynamic script injection.
    Distribution: Multiple posts with fake profit claims

    Execution: Users tricked into pasting as javascript: malicious code

    Obfuscation: Hexadecimal decoding reveals C2 servers

    Payload Retrieval: Fetches malicious script from remote servers

    Injection: Dynamic script execution with session privileges

    Impact: Session hijacking, transaction modification

Threat Actor Attribution

    OSINT operations across multiple platforms

    Blockchain forensic analysis and transaction tracing

    Threat actor profiling and pattern analysis

Detailed techniques: [OSINT Techniques](docs/osint-techniques.md) | [On-Chain Analysis](docs/On-chain.md)
🛡️ Mitigation & Impact
Security Recommendations

    CSP Hardening: Content Security Policy implementation

    WAF Rules: Custom rule development for injection detection

    Domain Blocking: Infrastructure takedown coordination

    User Protection: Proactive threat hunting recommendations

Key Achievements

    ✅ Direct attribution to threat actor operations

    ✅ Infrastructure takedowns through coordinated disclosures

    ✅ Formal recognition from affected organizations

    ✅ Thousands of users protected from financial loss

    ✅ Sector-wide IoC sharing preventing further attacks

🛠️ Technical Documentation [Methodoly](docs/methodology.md)

For detailed technical analysis, refer to these documents:

    Methodology: Complete investigation methodology

    JavaScript Analysis: Technical breakdown of malicious code

    OSINT Techniques: Open-source intelligence methods

    On-Chain Analysis: Blockchain investigation techniques

    Threat Intelligence: Campaign analysis and patterns

📊 Results & Impact

    3+ cryptocurrency exchanges protected

    Thousands of potential victims safeguarded

    100% infrastructure takedown success rate

    Formal recognition from affected organizations

    Ongoing monitoring established for related campaigns

🔒 Ethics & Security

    No PII stored in this repository

    No complete malicious domains included

    No executable malicious code present

    All content follows Responsible Disclosure guidelines

    Research conducted anonymously via Tor network

📧 Verification & Contact

Given the significant impact of this case in the crypto ecosystem, legitimate organizations, technical recruiters, or security teams may request:

    Additional technical information

    Identity verification and research authenticity

    Details about the applied methodology

Contact for legitimate verification:
blusterc@proton.me

This documentation serves educational and awareness purposes only. Any legal action should be conducted by competent authorities.
