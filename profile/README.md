<div align="center">

<img src="https://raw.githubusercontent.com/tiliondev/fortress/main/docs/assets/dockerhub-banner.png" width="100%">

# Tilion

**Stealth browser infrastructure for automation, testing, and large-scale data collection.**

We build browser engines that stay undetectable by moving fingerprint correction into the engine's **C++** — so a page inspecting itself sees stock Chromium. There is no JavaScript hijacking to detect.

</div>

---

## Open source

### 🏰 [Fortress](https://github.com/tiliondev/fortress) — stealth Chromium engine

Fingerprint spoofing compiled into Chromium's C++, driven by the Playwright or Puppeteer you already use. Every spoofed getter is native code, so `toString` returns `[native code]` identically across the main frame, iframes, and Web Workers. Clears **CreepJS**, **Sannysoft**, **BrowserScan**, and live **Cloudflare Turnstile** as a normal Chrome install.

[![GitHub](https://img.shields.io/badge/GitHub-tiliondev%2Ffortress-181717?logo=github)](https://github.com/tiliondev/fortress)
[![Docker Pulls](https://img.shields.io/docker/pulls/arham766/fortress?logo=docker&logoColor=white&label=docker%20pulls)](https://hub.docker.com/r/arham766/fortress)
[![Chromium](https://img.shields.io/badge/chromium-151-4285F4?logo=googlechrome&logoColor=white)](https://github.com/tiliondev/fortress)
[![License](https://img.shields.io/badge/license-BSD--3--Clause-blue)](https://github.com/tiliondev/fortress/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/tiliondev/fortress?style=social)](https://github.com/tiliondev/fortress/stargazers)

```bash
docker run --rm -p 9222:9222 arham766/fortress:latest        # raw CDP on :9222
pip install tilion-fortress                                  # Python SDK (Linux x64)
npm  install tilion-fortress                                 # Node SDK
```

- **Native-code parity** — realm-invariant getters, `[native code]` everywhere
- **Coherent by construction** — real V8, Blink, and BoringSSL keep engine, user-agent, and JA3/JA4 TLS in agreement
- **Auditable** — 34 single-surface C++ patches, reproducible from source, monthly Chromium rebase

---

<div align="center">
<sub>Stealth you can read, rebuild, and run yourself.</sub>
</div>
