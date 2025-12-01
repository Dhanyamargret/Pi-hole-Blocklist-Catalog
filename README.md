<!-- README.md -->

# Pi-hole Blocklist Catalog

![GitHub stars](https://img.shields.io/github/stars/PrimePoobah/Pi-hole-Blocklist-Catalog?style=flat-square)
![Last Updated](https://img.shields.io/github/last-commit/PrimePoobah/Pi-hole-Blocklist-Catalog?label=updated&style=flat-square)
![License](https://img.shields.io/badge/License-AGPL--3.0-orange?style=flat-square)
![Pi-hole v6 Compatible](https://img.shields.io/badge/Pi--hole-v6%20Compatible-brightgreen?style=flat-square)
![Curated Monthly](https://img.shields.io/badge/Curated-Monthly-blue?style=flat-square)

---

## 🎯 Why This Catalog Exists (Other Than My Poor Life Choices)

Welcome, digital freedom fighter.  
If you're here, you already know the pain: **finding good Pi-hole blocklists** is like digging through a dumpster behind a sketchy taco place.  
Some are outdated, some are broken, and some aggressively block your bank, your kid’s school portal, your cat's Instagram, and that one site you *claim* you don’t visit.

This repository exists to fix that mess.

Instead of blindly throwing 10+ random lists into Pi-hole and praying, this catalog focuses on:

- ✅ **High-quality, actively maintained** blocklists  
- ✅ **Clear categories** (ads, telemetry, malware, phishing, cryptomining, tracking, etc.)  
- ✅ **Realistic recommendations** for home, lab, and enterprise  
- ✅ **Reducing breakage** while still punching ads and malware in the face  

---

## 🧱 What This Catalog *Is* (And What It’s Not)

This catalog **is**:

- A curated list of trustworthy blocklists for **Pi-hole v6+** and similar DNS-based tools  
- A way to pick **sane defaults** without spending your weekend on forum archaeology  
- A living reference you can drop into docs, homelab wikis, and “please-fix-our-network” tickets  

This catalog is **not**:

- A “block the entire internet” collection  
- A magic bullet that guarantees *zero* breakage  
- A replacement for common sense (“maybe don’t deploy the nuclear malware list to Grandma’s iPad group”)  

---

## 📚 The Blocklist Catalog (The Good Stuff)

Looking for the actual list? Boom:

➡️ **[BLOCKLIST_CATALOG.md](./BLOCKLIST_CATALOG.md)**

Inside you’ll find:

- ✔ Validated for Pi-hole v6 compatibility, reachability, and recent maintenance signals  
- ✔ Proper categories (ads, trackers, telemetry, malware, and other internet gremlins)  
- ✔ Descriptions, reputation scores, and notes on false positives  
- ✔ Suggested use-cases (home, lab, SOC, admin devices, etc.)

If you just want a quick starting point for a **home Pi-hole**:

1. Pick **ONE** baseline:
   - `StevenBlack Unified Hosts` **or**  
   - `Hagezi Multi Normal` **or**  
   - `OISD Small` **or**  
   - `1Hosts (Lite)`

2. Add a **malware/phishing layer**:
   - `URLHaus Hostfile`  
   - `ThreatFox Hostfile`  
   - Optionally one of the more aggressive lists if you like living dangerously

3. If you’re on Windows-heavy networks and enjoy telemetry-free vibes:
   - Consider the **telemetry lists** (in their own section) **via Pi-hole groups only**.

---

## 🧪 Compatibility

These lists are designed for:

- **Pi-hole v6+** (hosts & domain lists)  
- DNS-based firewalls & filters:
  - Unbound  
  - AdGuard Home  
  - pfBlockerNG  
  - Router-level DNS filtering (where compatible)

Each entry in the catalog includes:

- URL  
- Category  
- Maintainer  
- Approximate reputation score  
- Notes about aggressiveness, best use-cases, and gotchas  

---

## ⚠️ Use With Care (a.k.a. Don’t Blame Me For Your Broken Netflix)

Some lists are **very** aggressive. That’s great for:

- Admin workstations  
- Security labs  
- SOC environments  

It’s… less great for:

- Family iPads  
- Smart TVs that already barely function  
- That one teacher who definitely will email if anything breaks

Use **Pi-hole groups**:

- Keep a sane baseline for everyone  
- Assign aggressive malware/telemetry lists only to the devices that need them  
- Whitelist sparingly and intentionally  

---

## 🧾 License

This repo is licensed under:

> **GNU Affero General Public License v3.0 (AGPL-3.0)**

Because if we’re going to share the pain and joy of blocklists, we might as well do it the open-source way.

---

## ⭐ Support This Madness

If you found this helpful—or mildly entertaining—drop a ⭐ on the repo.

It helps more Pi-hole users:

- Improve privacy  
- Block the bad guys  
- Break fewer websites  
- And appreciate that sarcasm belongs in tech docs  

Thanks for stopping by, you magnificent bandwidth-saving champion.
