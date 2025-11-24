# ⛓️ On-Chain Analysis & Blockchain Forensics

## Objective
Trace cryptocurrency transactions associated with the malicious campaign through mixing services and identify financial patterns for attribution.

## Tools & Platforms
**Blockchain Explorers**
- Blockchair  
- Blockchain.com  
- Etherscan  
- WalletExplorer.com  
- OXT.me  

**Tracked Wallet Software**
- Cake Wallet  
- Wasabi Wallet  
- JoinMarket  
- *Redacted*: “Bl*** Py***mid” wallet/service and Illegal Mixer

**Analysis Tooling**
- Custom Python scripts (pandas, NetworkX)
- Transaction graph builders
- API integrations for data retrieval

**Data Sources**
- Public blockchain data  
- Exchange APIs  
- Archived transaction datasets  

---

## Methodology

### 1. Address Clustering
Applied **common-input-ownership** and **change address heuristics** to group linked Bitcoin addresses.

Techniques used:
- Multi-input heuristic  
- Change-output detection  
- Address-type consistency (P2PKH / P2SH / Bech32)  
- Cluster merging via transaction graph connectivity  

Result:  
**42 addresses** attributed to 3 operational clusters.

---

### 2. Mixer Detection & Tracing

**CoinJoin / Wasabi / JoinMarket Indicators**
- Equalized output amounts  
- CoinJoin multisig patterns  
- Round-based batching  
- Coordinated timing windows  

**Deobfuscation Techniques**
- Pre/Post-mix timing correlation  
- Fee-pattern normalization  
- Graph traversal across multi-hop paths  
- Cross-referencing known mixer fingerprints (OXT heuristics + WalletExplorer labels)

---

### 3. Behavioral Analysis

**Temporal Analysis**
- Recurrent activity between **14:00–20:00 UTC**
- Burst transactions before cash-out events

**Amount Analysis**
- Strict operational preference for **0.1 BTC batches**
- Occasional consolidation into **0.25–0.5 BTC** for withdrawals

**Exchange Interaction**
- Identification of preferred exchanges via deposit address clustering
- Repeated deposit behavior consistent over multiple weeks

---

## Key Findings

### Financial Flow Mapping
- **₂.1 BTC** traced through mixing infrastructure  
- **3 primary operational wallets** linked with high confidence  
- Full movement path mapped:  
  **Source → Mixing → Post-mix cluster → Exchange cash-out**  
- Estimated **₿0.15 BTC** in mixing fees  

---

## Attribution Indicators

### High-Confidence Evidence
- Stable transaction timing rhythms  
- Consistent fee preferences  
- Unique batching structure  
- Repeated reliance on identical mixers  
- Multi-hop graph structure matching OSINT-identified behavior  

### Operational Mistakes Identified
The threat actor was successfully traced due to:
- Not using privacy-focused chains (Monero, Firo, PIVX, Pirate Chain)
- Not using Tornado Cash for ETH  
- Poor mixing hygiene (reused address patterns, timing leaks)
- Predictable consolidation habits

---

## Conclusion
The on-chain analysis reveals a consistent financial pattern enabling high-confidence clustering and attribution. Despite the use of mixing tools, predictable behaviors, fee patterns, and timing correlations exposed the actor’s full transactional flow.

