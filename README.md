# 🦉 ONexusX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **ONexusX** — Sonatype Nexus Repository Manager Config Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Sonatype Nexus Repository Manager configuration security auditor

---

## ✨ Features

- Stdlib parsers — Java .properties, Jetty XML, JSON / XML exports, nginx.conf, .vmoptions
- nexus.properties / nexus-default.properties — nexus-args TLS, application-host, scripts creation, random admin password, anti-CSRF, H2 / Orient listeners, datastore credentials
- Jetty jetty-https.xml / jetty.xml — protocols, cipher suites, keystore passwords, server version
- Realm order, anonymous access, LDAP / SAML / Crowd
- Repository exports — hosted / proxy / group, Docker connectors, dependency confusion, routing
- Blobstore & $data-dir permission walk, soft quota
- Secrets masked everywhere; --root discovery; CWE + MITRE
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Self-test --demo, CI gates --fail-on / --min-severity

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ONexusX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
