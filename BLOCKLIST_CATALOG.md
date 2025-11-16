# 🛡️ Pi-hole Blocklist Catalog

Curated, **Pi-hole v6+ compatible** blocklists from reputable, actively maintained sources.  
All lists are:

- 🌐 Served via **HTTPS**  
- 🧱 Hosts / Domain / Adblock compatible  
- 🔄 Actively maintained (≤12–18 months)  
- 🧪 Generally low false-positives (but always test)

---

## 🔎 Quick Navigation

- [Legend](#-legend)
- [Recommended Baseline Lists](#-recommended-baseline-lists)
- [Ads](#-ads)
- [Adult](#-adult)
- [Crypto](#-crypto)
- [Malware](#-malware)
- [Mixed](#-mixed)
- [Phishing](#-phishing)
- [Suspicious / Threat-Intel](#-suspicious--threat-intel)
- [Telemetry](#-telemetry)
- [Tracking / CNAME Cloaking](#-tracking--cname-cloaking)
- [Implementation Notes](#-implementation-notes)

---

## 🧾 Legend

- **Reputation Score (Rep)**  
  - 10 – elite, widely trusted, mature  
  - 8–9 – strong, reliable, actively maintained  
  - 6–7 – good but aggressive or niche  

- **🆕 NEW** — newly added based on your active Pi-hole configuration

---

# ⭐ Recommended Baseline Lists  
*(Choose ONE as your main daily-driver list)*

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| **StevenBlack Unified Hosts** | [link](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts) | ads, malware, suspicious, tracking | Long-standing unified blocklist combining curated reputable sources. | Steven Black | Very active | **10/10** | ~110k | Excellent stability, trusted worldwide. |
| **Hagezi Multi Normal** | [link](https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/multi.txt) | ads, malware, phishing, suspicious, telemetry, tracking | Balanced, high-quality multipurpose blocklist. | Hagezi | Active | **10/10** | ~267k | Great all-around baseline. |
| **OISD Small** | [link](https://small.oisd.nl) | ads, malware, tracking, telemetry | Clean, curated, small & stable. | OISD | Active | **10/10** | ~71k | Minimal breakage, ideal for home/school networks. |

---

# 📢 Ads

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| AdAway Hosts 🆕 NEW | [link](https://adaway.org/hosts.txt) | ads, tracking | Classic mobile-focused adblocking list. | AdAway | Active | 9/10 | — | Strong, low false-positives. |
| Disconnect Simple Ads 🆕 NEW | [link](https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt) | ads | Clean, high-quality adblock list. | Disconnect | Active | 9/10 | — | Great companion to baseline lists. |
| Disconnect Malvertising 🆕 NEW | [link](https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt) | ads, malware | Blocks malicious ad/malvertising domains. | Disconnect | Active | 9/10 | — | Good malware supplement. |
| RPiList EasyList Extended | [link](https://raw.githubusercontent.com/RPiList/specials/master/Blocklisten/easylist) | ads, tracking | DNS version of EasyList. | RPiList | Active | 8/10 | — | Moderately aggressive. |

---

# 🔞 Adult

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| OISD NSFW | [link](https://nsfw.oisd.nl) | adult, ads, tracking | Adult-content blocking variant of OISD. | OISD | Active | 9/10 | — | Use ethically where required. |

---

# 🪙 Crypto

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| BlocklistProject Crypto | [link](https://raw.githubusercontent.com/blocklistproject/Lists/master/crypto.txt) | crypto, suspicious | Blocks malicious mining & crypto scams. | BlocklistProject | Active | 8/10 | — | Best for high-risk groups. |
| Prigent Crypto 🆕 NEW | [link](https://v.firebog.net/hosts/Prigent-Crypto.txt) | crypto, suspicious | Crypto-abuse & mining domains. | Prigent | Active | 8/10 | — | Optional supplement. |

---

# 🦠 Malware

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| URLHaus Hostfile | [link](https://urlhaus.abuse.ch/downloads/hostfile/) | malware, phishing, suspicious | Actively updated malware distribution domains. | abuse.ch | Multiple times daily | **10/10** | — | One of the best malware feeds. |
| ThreatFox Hostfile | [link](https://threatfox.abuse.ch/downloads/hostfile/) | malware, phishing, suspicious | C2/payload/malware infra from global IOCs. | abuse.ch | Rolling updates | 9/10 | — | High-signal threat feed. |
| RPiList Malware | [link](https://raw.githubusercontent.com/RPiList/specials/master/Blocklisten/malware) | malware | Maintained malware list. | RPiList | Active | 8/10 | — | Good supplement. |
| OSINT.digitalside.it LatestDomains 🆕 NEW | [link](https://osint.digitalside.it/Threat-Intel/lists/latestdomains.txt) | malware, suspicious | OSINT-driven daily malware/TI domains. | DigitalSide | Daily | 9/10 | — | Excellent modern TI feed. |
| FadeMind Risk Hosts 🆕 NEW | [link](https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Risk/hosts) | malware, suspicious | Risky/abusive domains curated via OSINT. | FadeMind | Active | 8/10 | — | More aggressive. |
| DandelionSprout Anti-Malware 🆕 NEW | [link](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Alternate%20versions%20Anti-Malware%20List/AntiMalwareHosts.txt) | malware | Community anti-malware list. | DandelionSprout | Active | 8/10 | — | Solid optional list. |
| NoTrack Malware (quidsup) 🆕 NEW | [link](https://gitlab.com/quidsup/notrack-blocklists/raw/master/notrack-malware.txt) | malware | Malware list from NoTrack. | quidsup | Mostly active | 7/10 | — | Optional. |

---

# 🧩 Mixed

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| Hagezi Multi Pro | [link](https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/pro.txt) | ads, malware, phishing, suspicious | Aggressive variant of Multi Normal. | Hagezi | Active | 8/10 | ~354k | Best in separate group. |
| OISD Big | [link](https://big.oisd.nl) | ads, malware, phishing, suspicious | Large mega-list with huge coverage. | OISD | Active | 9/10 | ~438k | Heavy. Monitor logs. |

---

# 🎣 Phishing

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| BlocklistProject Phishing | [link](https://raw.githubusercontent.com/blocklistproject/Lists/master/phishing.txt) | phishing | Credential phishing & scam domains. | BlocklistProject | Active | 9/10 | — | Consistent & clean. |
| Phishing Army (Extended) 🆕 NEW | [link](https://phishing.army/download/phishing_army_blocklist_extended.txt) | phishing | Expanded phishing feed with broader coverage. | Phishing Army | Daily | 9/10 | — | Recommended version. |

---

# ⚠️ Suspicious / Threat-Intel

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| BlocklistProject Ransomware | [link](https://raw.githubusercontent.com/blocklistproject/Lists/master/ransomware.txt) | malware, suspicious | Ransomware-related infra & payment portals. | BlocklistProject | Active | 8/10 | — | Low noise. |
| BlocklistProject Scam | [link](https://raw.githubusercontent.com/blocklistproject/Lists/master/scam.txt) | phishing, suspicious | Fake shops, fraud, refund scams. | BlocklistProject | Active | 8/10 | — | Good “general safety” layer. |
| Hagezi TIF | [link](https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/tif.txt) | malware, phishing, suspicious | High-risk threat feed. | Hagezi | Active | 9/10 | — | Use for admin/high-risk devices. |

---

# 📡 Telemetry

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| RPiList Win10 Telemetry | [link](https://raw.githubusercontent.com/RPiList/specials/master/Blocklisten/Win10Telemetry) | telemetry, tracking | Blocks Windows telemetry & tracking endpoints. | RPiList | Active | 8/10 | — | May break MS cloud features. |

---

# 📍 Tracking / CNAME Cloaking

| Name | URL | Categories | Description | Maintainer | Updated | Rep | Entries | Notes |
|------|-----|------------|-------------|------------|---------|-----|---------|-------|
| Frogeye First-Party Trackers 🆕 NEW | [link](https://hostfiles.frogeye.fr/firstparty-trackers-hosts.txt) | tracking | Detects 1st-party & CNAME-cloaked trackers. | Frogeye | Active | **10/10** | — | Highly effective modern tracking list. |

---

# 🛠 Implementation Notes

## Recommended Setup for Most Networks

**Choose ONE baseline list:**

- ⭐ StevenBlack Unified Hosts  
- ⭐ Hagezi Multi Normal  
- ⭐ OISD Small  

**Add core security feeds:**

- 🦠 URLHaus  
- 🕵️ ThreatFox  
- 🎣 Phishing Army (Extended)  
- 📍 Frogeye First-Party Trackers  

**Optional (based on environment):**

- 🔞 OISD NSFW  
- 🔥 Hagezi Multi Pro / TIF  
- 🪙 Crypto lists  
- 🪟 Windows telemetry lists  

---

## Pi-hole v6+ Group Strategy

- Create **strict/security groups** for:  
  - URLHaus  
  - ThreatFox  
  - Hagezi TIF  
  - Hagezi Multi Pro  
  - OISD Big  
  - OSINT.digitalside  

- Apply strict groups only to:  
  - Admin devices  
  - High-risk devices  
  - Lab/test clients  

---

_“Updated” values and entry counts are estimates based on most recent public data as of 2024–2025._

