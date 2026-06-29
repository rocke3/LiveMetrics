<div align="center">

<img src="https://net.mdrashid.com/logo-192.png" width="96" height="96" alt="LiveMetrics app icon">

# LiveMetrics

### Your whole Mac, in the menu bar.

Free, native macOS menu-bar **network + system monitor**. Live upload/download speed plus CPU, GPU, RAM, temperatures, disk, fans and power — every second, right where you glance.

[![macOS 14+](https://img.shields.io/badge/macOS-14%2B-111111?logo=apple&logoColor=white)](https://net.mdrashid.com/)
[![Price](https://img.shields.io/badge/price-free-22C55E)](https://net.mdrashid.com/)
[![Signed & notarized](https://img.shields.io/badge/signed%20%26%20notarized-by%20Apple-3B82F6)](https://net.mdrashid.com/)
[![Size](https://img.shields.io/badge/download-~1.4%20MB-6366F1)](https://net.mdrashid.com/LiveMetrics.dmg)

### [⬇️ Download for macOS](https://net.mdrashid.com/LiveMetrics.dmg) · [Website](https://net.mdrashid.com/)

<br>

<img src="https://net.mdrashid.com/livemetrics-social-banner.png" width="800" alt="LiveMetrics — live network speed plus CPU, GPU, RAM, temperature, disk, fans and power in the macOS menu bar">

</div>

---

## What it does

LiveMetrics puts your Mac's vitals in the menu bar so you never open a window to check them.

- **Live network speed** — ↓ download and ↑ upload, refreshed every second, with today's peak and a rolling graph (1–30 min window).
- **CPU, GPU, RAM, temperature** — pinned to the menu bar by default.
- **Disk, fans, and power draw in watts** — optional swaps, one click away.
- **Compact colored chips** in the menu bar; each metric also gets a live popover card with a 5-minute sparkline.
- **Auto-scaling units** — bytes (KB/s, MB/s) or bits (Kb/s, Mb/s).

At most 6 system metrics fit in the menu bar at once — every chip is customizable.

## Screenshot

<div align="center">

<img src="https://net.mdrashid.com/app-preview.jpg" width="420" alt="LiveMetrics popover in the macOS menu bar showing live upload and download speed, a rolling throughput graph, and CPU, GPU, RAM, disk and temperature cards">

<br><em>The LiveMetrics popover — live ↑/↓ speed, today's peak, a rolling graph, and CPU, GPU, RAM, disk and temperature cards.</em>

</div>

## Not a speed test

A speed test runs once and generates traffic to measure a maximum. LiveMetrics is a **passive bandwidth monitor**: it reads your Mac's own interface byte counters, so the numbers reflect the real traffic already flowing through your connection — second by second, with nothing to run.

## Private by design

Reads everything **locally** from `getifaddrs()`, IOKit/mach, and the Apple SMC. No kernel extension, no admin rights, no Terminal. No accounts, no analytics, no tracking — **nothing leaves your Mac.**

## Install

1. [Download the `.dmg`](https://net.mdrashid.com/LiveMetrics.dmg) (~1.4 MB).
2. Drag **LiveMetrics** to your Applications folder, then open it.
3. It's **signed & notarized by Apple** (Developer ID: palmy llc), so it opens with a normal double-click — if macOS asks to confirm the download, click **Open**.

It updates itself automatically. **Requirements:** macOS 14 (Sonoma) or later · Apple Silicon and Intel.

## A free iStat Menus alternative

| | LiveMetrics | iStat Menus | Stats (exelban) | Activity Monitor |
|---|:---:|:---:|:---:|:---:|
| Price | **Free** | ~$11.99 | Free, open-source | Free (built in) |
| Network speed in menu bar | ✅ | ✅ | ✅ | ❌ |
| CPU / GPU / RAM | ✅ | ✅ | ✅ | Window only |
| Temps / fans | ✅ | ✅ | ✅ | ❌ |
| Power draw (watts) | ✅ | ✅ | ✅ | ❌ |
| Footprint | ~1.4 MB | Full suite | Full suite | System app |

LiveMetrics is the lightweight free option for the everyday essentials. iStat Menus goes deeper (longer history, per-process detail, more sensors).

## Links

- 🌐 Website — https://net.mdrashid.com/
- ⬇️ Download — https://net.mdrashid.com/LiveMetrics.dmg
- 📘 How to show network speed in the Mac menu bar — https://net.mdrashid.com/how-to-show-network-speed-mac-menu-bar
- 🔍 Free iStat Menus alternative — https://net.mdrashid.com/free-istat-menus-alternative-mac
- ⚡ Free Mac menu-bar watts / power monitor — https://net.mdrashid.com/free-mac-menu-bar-watts-power-monitor
- ⚖️ LiveMetrics vs Stats — https://net.mdrashid.com/livemetrics-vs-stats

---

Built by [Mamunur Rashid](https://mdrashid.com/) — an independent developer making small, focused, privacy-respecting tools for macOS, the browser, and the editor. Feedback and feature requests welcome via [Issues](https://github.com/rocke3/LiveMetrics/issues).
