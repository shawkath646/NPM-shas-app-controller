<!-- HEADER SECTION -->
<div align="center">

# SHAS App Controller (`shas-app-controller`)

**[DEPRECATED] Next.js npm package for remote project activation, deactivation, and alert toasts.**

<!-- BADGES -->
[![Status](https://img.shields.io/badge/Status-Deprecated-inactive?style=flat-square)](#)
[![Author](https://img.shields.io/badge/Author-Shawkat%20Hossain%20Maruf-black?style=flat-square)](https://shawkath646.dev)
[![Ecosystem](https://img.shields.io/badge/Ecosystem-clouburstlab-2563EB?style=flat-square)](https://clouburstlab.com)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](#-license)
[![NPM](https://img.shields.io/badge/NPM-shas--app--controller-CB3837?style=flat-square&logo=npm&logoColor=white)](#)

</div>

---

### 📋 Project Overview

| Property | Details |
| :--- | :--- |
| **Author** | [Shawkat Hossain Maruf](https://shawkath646.dev) |
| **Platform** | Node.js / NPM Library (Next.js Application Controller) |
| **Period / Timeline** | Mar 2024 |
| **Status** | Deprecated / Unmaintained (Archived) |
| **Origin** | Evolved from [`sh-web-switch`](https://github.com/shawkath646/sh-web-switch) |
| **Primary Stack** | TypeScript, Next.js, NPM Package |

---

> [!WARNING]
> **Deprecation Notice**  
> This package is **deprecated, unmaintained, and archived**. It was built as the package-based successor to [`sh-web-switch`](https://github.com/shawkath646/sh-web-switch) to integrate with the legacy **SH Authentication System (SHAS)**. Both tools are now legacy and preserved solely for archival purposes.

---

## 🎯 Purpose & History

### Why It Existed
Developed to eliminate the need for hardcoded remote controls, this module connected Next.js applications directly to the central SH Authentication System dashboard. It allowed the site owner to remotely deactivate applications, fetch registered brand metadata, and display dynamic maintenance toast alerts without re-deploying code.

### What It Solved
- **No-Code Remote Kill-Switch:** Handled project status queries dynamically during Next.js server-side rendering.
- **Broadcast Alert Toasts:** Delivered global maintenance and warning banners into consumer frontends with configurable recurrence intervals.
- **Metadata Synchronization:** Automatically synchronized application name, logos, and support contacts registered in SHAS.

---

## 📦 Historical Usage (Legacy Reference)

```bash
npm install --save-dev shas-app-controller
```

### Configuration (`shas.config.ts`)

```typescript
import SHAS from "shas-app-controller";

const { ContentWrapper, appData, brandData } = await SHAS({
  appId: process.env.SHAS_APP_ID as string,
  appSecret: process.env.SHAS_APP_SECRET as string,
  cache: "no-cache",
  toastReminder: 86400 // Reappear interval in seconds
});
```

---

## 🛠️ Tech Stack & Dependencies

- **Language:** TypeScript
- **Target Runtime:** Node.js / Next.js
- **Ecosystem:** Legacy SHAS (SH Authentication System)

---

## 📄 License

Distributed under the [MIT License](LICENSE). See `LICENSE` for more information.

---

<!-- BRANDING FOOTER -->
<div align="center">
  <sub>Engineered by</sub><br/>
  <strong><a href="https://shawkath646.dev">Shawkat Hossain Maruf</a></strong>
  <br/><br/>
  <sub>A product of</sub><br/>
  <a href="https://clouburstlab.com" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://assets.clouburstlab.com/branding/icon_dark.png">
      <source media="(prefers-color-scheme: light)" srcset="https://assets.clouburstlab.com/branding/icon_light.png">
      <img alt="clouburstlab" src="https://assets.clouburstlab.com/branding/icon_light.png" width="230">
    </picture>
  </a>
</div>
