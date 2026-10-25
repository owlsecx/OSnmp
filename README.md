# 🦉 OSnmp

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OSnmp** — SNMP Scanner & Exploitation Suite

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview


OSnmp is an SNMP scanner and exploitation suite built for fast, parallel assessment of SNMP-enabled devices. It performs quick scans, community-string brute forcing, OID walks, system enumeration and single-OID gets, all with a threaded engine and stdlib-only implementation. It is intended for authorized purple-team and penetration-testing work.

---

## ✨ Features


- Ultra-fast parallel SNMP scanning with a configurable thread pool
- Community-string brute force from a built-in default or a supplied wordlist
- OID walk, system enumeration and single-OID get modes
- Multiple scan modes including a full scan (brute + sysinfo + walk)
- Configurable port, timeout and output file, with export of last results
- Pure stdlib (no external dependencies); --self-test for offline verification

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./OSnmp -t 192.168.1.10 -m quick
./OSnmp -t 10.0.0.0/24 --communities wordlist.txt -m brute --threads 100
./OSnmp --single-get 192.168.1.10 public 1.3.6.1.2.1.1.1.0
./OSnmp --self-test
./OSnmp --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
