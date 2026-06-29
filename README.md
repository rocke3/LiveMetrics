<div align="center">

<img src="https://net.mdrashid.com/logo-192.png" width="96" height="96" alt="LiveMetrics app icon">

# LiveMetrics

### Your whole Mac, in the menu bar.

Free, native **macOS menu bar network + system monitor**. Live upload/download speed plus CPU, GPU, RAM, temperatures, disk, fans and power draw — every second, right where you glance.

[![macOS 14+](https://img.shields.io/badge/macOS-14%2B-111111?logo=apple&logoColor=white)](https://net.mdrashid.com/)
[![Price](https://img.shields.io/badge/price-free-22C55E)](https://net.mdrashid.com/)
[![Signed & notarized](https://img.shields.io/badge/signed%20%26%20notarized-by%20Apple-3B82F6)](https://net.mdrashid.com/)
[![Size](https://img.shields.io/badge/download-~1.4%20MB-6366F1)](https://net.mdrashid.com/LiveMetrics.dmg)

### [⬇️ Download for macOS](https://net.mdrashid.com/LiveMetrics.dmg) · [Website](https://net.mdrashid.com/)

<br>

<img src="https://net.mdrashid.com/livemetrics-social-banner.png" width="800" alt="LiveMetrics — live network speed plus CPU, GPU, RAM, temperature, disk, fans and power in the macOS menu bar">

</div>

---

**LiveMetrics is a free, native macOS app that shows live network speed in the Mac menu bar** — upload and download updated every second — and ships as a full system monitor with CPU, GPU, RAM and temperature pinned by default, plus optional disk, fans and live power draw in watts. It is a passive bandwidth monitor (not a speed test), reads everything locally with no kernel extension, and is a lightweight free alternative to iStat Menus and Stats.

**Contents:** [What it is](#what-is-livemetrics) · [Features](#features) · [Show network speed in the menu bar](#how-to-show-network-speed-in-the-mac-menu-bar) · [Free iStat Menus alternative](#a-free-istat-menus-alternative) · [Live watts / power monitor](#live-power-monitor-watts) · [How it works](#how-it-works) · [Privacy](#privacy) · [FAQ](#faq)

---

## What is LiveMetrics?

LiveMetrics is a **menu bar system monitor for macOS**. macOS has no built-in way to show your network speed in the menu bar, and Activity Monitor only lives in a window or the Dock. LiveMetrics fills that gap: it puts a readable upload/download number — and the rest of your Mac's vitals — next to the clock, so you never open a window to check them.

- **Network:** live ↓ download and ↑ upload speed, today's peak, and a rolling graph (1–30 min window).
- **System (pinned by default):** CPU, GPU, RAM and temperature.
- **System (optional swaps):** disk throughput, fan RPM, and live power draw in watts.
- **Tiny & native:** ~1.4 MB Swift/SwiftUI agent app, no Dock icon, sips CPU.

## Features

| | |
|---|---|
| 🌐 **Network speed** | Live ↑/↓ in the menu bar, refreshed every second; today's peak; rolling Swift Charts graph; bytes or bits units |
| 🧠 **CPU** | Overall % and per-core, user/system split |
| 🎮 **GPU** | Utilization % with GPU name (Intel, AMD, Apple Silicon) |
| 💾 **RAM** | Used %, used/total, macOS memory pressure, compressed + swap |
| 🌡️ **Temperature** | CPU/GPU/RAM sensors via the Apple SMC, °C or °F |
| 💽 **Disk** | Read/write throughput (optional) |
| 🌀 **Fans** | Per-fan RPM, or "Fanless" (optional) |
| ⚡ **Power** | Live watts — per-domain SoC power on Apple Silicon (optional) |

Up to 6 system metrics fit in the menu bar at once as compact colored chips; each also gets a popover card with a 5-minute sparkline. Every chip is customizable — turn any default off, or swap in disk, fans or power.

## Screenshot

<div align="center">

<img src="https://net.mdrashid.com/app-preview.jpg" width="420" alt="LiveMetrics popover in the macOS menu bar showing live upload and download speed, a rolling throughput graph, and CPU, GPU, RAM, disk and temperature cards">

<br><em>The LiveMetrics popover — live ↑/↓ speed, today's peak, a rolling graph, and CPU, GPU, RAM, disk and temperature cards.</em>

</div>

## How to show network speed in the Mac menu bar

1. [**Download LiveMetrics**](https://net.mdrashid.com/LiveMetrics.dmg) — a free ~1.4 MB disk image (.dmg).
2. **Drag LiveMetrics to your Applications folder**, then open it.
3. **That's it** — live upload and download speed now appear in your menu bar, updated every second.
4. *Optional:* enable **Launch at Login** so it's always there.

It's **signed and notarized by Apple** (Developer ID: palmy llc), so it opens with a normal double-click — if macOS asks to confirm the download, click **Open**. No right-click trick, no Terminal, no App Store account. It updates itself automatically.

**Requirements:** macOS 14 (Sonoma) or later · Apple Silicon and Intel.

📘 Full guide: [How to show network speed in the Mac menu bar](https://net.mdrashid.com/how-to-show-network-speed-mac-menu-bar)

## A free iStat Menus alternative

Looking for a **free iStat Menus alternative**? LiveMetrics covers the core menu-bar metrics — network, CPU, GPU, RAM, disk, temperatures, fans and power — for free, in a ~1.4 MB download.

| | LiveMetrics | iStat Menus | Stats (exelban) | Activity Monitor |
|---|:---:|:---:|:---:|:---:|
| Price | **Free** | ~$11.99 one-time | Free, open-source | Free (built in) |
| Network speed in menu bar | ✅ | ✅ | ✅ | ❌ (window/Dock only) |
| CPU / GPU / RAM | ✅ | ✅ | ✅ | Window only |
| Temperatures / fans | ✅ | ✅ | ✅ | ❌ |
| Power draw (watts) | ✅ | ✅ | ✅ | ❌ |
| Rolling graph (up to 30 min) | ✅ | ✅ | ✅ | Limited |
| History, notifications, per-process | — | ✅ (deeper) | Partial | Process list |
| Footprint | **~1.4 MB** | Full suite | Full suite | System app |

LiveMetrics is the lightweight free option for the everyday essentials. iStat Menus goes deeper (longer history, per-process detail, more sensors); Stats is the free open-source full suite. 🔍 Compare: [free iStat Menus alternative](https://net.mdrashid.com/free-istat-menus-alternative-mac) · [LiveMetrics vs Stats](https://net.mdrashid.com/livemetrics-vs-stats)

## Live power monitor (watts)

macOS never shows how many **watts** your Mac is drawing — Activity Monitor's "Energy Impact" is a relative score, not a wattage. LiveMetrics adds an optional **live watts chip** to the menu bar. On Apple Silicon it reads **per-domain SoC power** (CPU, GPU, Neural Engine, RAM) from Apple's IOReport "Energy Model" group, plus whole-machine draw from the battery when unplugged — root-free, no kernel extension. ⚡ More: [free Mac menu-bar watts / power monitor](https://net.mdrashid.com/free-mac-menu-bar-watts-power-monitor)

## How it works

LiveMetrics is a **passive monitor, not a speed test**. A speed test runs once and generates traffic to a remote server to report a maximum; LiveMetrics runs continuously and reads counters your Mac already maintains, so the numbers reflect the real traffic already flowing through your connection.

- **Network:** polls `getifaddrs()` once per second on a background timer, sums the byte counters across active interfaces, and computes `delta / elapsed`. Counter wraps are clamped to 0.
- **CPU / GPU / RAM:** read from IOKit/mach.
- **Temperatures / fans:** read from the **Apple SMC**.
- **Power:** read from the **IOReport** "Energy Model" group on Apple Silicon.

No sockets are opened, no traffic is generated, and no admin rights, kernel extension, or `sudo` are required.

## Privacy

LiveMetrics reads **only local interface and sensor statistics** and sends nothing off your device. No accounts, no analytics, no tracking — nothing leaves your Mac.

## FAQ

### Is LiveMetrics free?
Yes. LiveMetrics is a completely free macOS app, distributed as a direct `.dmg` download. No account, no trial, no subscription.

### How do I show network speed in the Mac menu bar?
Download and open LiveMetrics. It places live upload and download speed in your menu bar automatically, updated every second. Enable Launch at Login so it is always there when you start your Mac.

### Is LiveMetrics a good free iStat Menus alternative?
Yes, for the essentials. It covers network, CPU, GPU, RAM, disk, temperatures, fans and power in the menu bar for free in a ~1.4 MB app. iStat Menus is paid and goes deeper (longer history, per-process detail, more sensors).

### Can it show CPU temperature and other system stats in the menu bar?
Yes — out of the box. CPU, GPU, RAM and temperature are pinned by default; disk, fans and power are optional swaps. Temperatures are read from the Apple SMC in °C or °F, with no kernel extension or admin password.

### Can LiveMetrics show how many watts my Mac is using?
Yes, on Apple Silicon. The optional power chip shows live per-domain SoC power (CPU, GPU, Neural Engine, RAM) in watts, read from Apple's IOReport — no Terminal or kernel extension.

### Is LiveMetrics a speed test?
No. It is a passive bandwidth monitor that reports the real throughput already flowing through your Mac, second by second, with nothing to run.

### Does macOS block it on first launch?
No. LiveMetrics is signed and notarized by Apple, so it opens with a normal double-click; macOS may just ask you to confirm the download once.

### What are the system requirements?
macOS 14 (Sonoma) or later, on Apple Silicon or Intel Macs.

## Why I built it

LiveMetrics started as a single speed readout next to my clock — macOS had no built-in way to show it — and grew into a full system monitor only because I kept wanting more of my Mac's vitals there myself. It's built to do one thing well and stay out of your way.

## Links

- 🌐 **Website** — https://net.mdrashid.com/
- ⬇️ **Download (.dmg)** — https://net.mdrashid.com/LiveMetrics.dmg
- 📘 **How to show network speed in the Mac menu bar** — https://net.mdrashid.com/how-to-show-network-speed-mac-menu-bar
- 🔍 **Free iStat Menus alternative for Mac** — https://net.mdrashid.com/free-istat-menus-alternative-mac
- ⚡ **Free Mac menu-bar watts / power monitor** — https://net.mdrashid.com/free-mac-menu-bar-watts-power-monitor
- ⚖️ **LiveMetrics vs Stats (exelban)** — https://net.mdrashid.com/livemetrics-vs-stats

---

Built by [**Mamunur Rashid**](https://mdrashid.com/) — an independent developer making small, focused, privacy-respecting tools for macOS, the browser, and the editor (also [TabAutopilot](https://chromewebstore.google.com/detail/nplekjmldglpfcdiechmgahoefhfheom) for Chrome and [NPM Manager](https://marketplace.visualstudio.com/items?itemName=MdRashid.npm-manager) for VS Code). Feedback and feature requests welcome via [Issues](https://github.com/rocke3/LiveMetrics/issues).

*LiveMetrics v1.2 · Updated June 2026 · macOS 14+ · Free*
