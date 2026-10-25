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

ONexusX is an offline, read-only Sonatype Nexus Repository Manager configuration auditor. It parses nexus.properties, Jetty HTTPS XML, datastore/realm exports, LDAP/SAML/Crowd settings, repositories, blobstores, and optional nginx frontends. Secrets are masked; findings map to CWE and MITRE ATT&CK with multi-format export and CI gates.

---

## ✨ Features

- Stdlib parsers for Java .properties, Jetty XML, JSON/XML exports, nginx.conf, and .vmoptions
- nexus.properties review: TLS args, application-host, scripts creation, admin password, anti-CSRF, H2/Orient, datastore credentials
- Jetty HTTPS protocols, cipher suites, keystore passwords, and server version checks
- Realm order, anonymous access, LDAP / SAML / Crowd configuration review
- Repository exports (hosted/proxy/group, Docker connectors, dependency confusion) and blobstore permission walk
- Secret masking, `--root` discovery, TXT/MD/JSON/CSV/SARIF export, `--demo` and fail-on gates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ONexusX /opt/sonatype/nexus --scan
./ONexusX --file nexus.properties --nginx nexus.conf -f json -o nexus.json
./ONexusX --demo --fail-on high
./ONexusX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
