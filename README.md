<div align="center">

# ☕ CNTCafé Public Configs

**Free, automatically-tested V2Ray / Xray proxy configs — refreshed every few hours.**
VLESS · VMess · Trojan · Shadowsocks · Hysteria2 — for V2rayNG, NekoBox, Hiddify, Streisand, Clash Meta & more.

[![Live](https://img.shields.io/badge/status-live%20%26%20auto--updated-brightgreen)](https://github.com/CNT-Cafe/Public-Configs)
[![Configs](https://img.shields.io/badge/configs-200%20working-blue)](https://github.com/CNT-Cafe/Public-Configs/blob/main/test-configs.txt)
[![Protocols](https://img.shields.io/badge/protocols-VLESS%20%C2%B7%20VMess%20%C2%B7%20Trojan%20%C2%B7%20SS%20%C2%B7%20Hysteria2-orange)](https://github.com/CNT-Cafe/Public-Configs)

[📥 **Subscribe**](#-subscription-links) · [❓ FAQ](#-faq) · [📡 Telegram](https://t.me/CNTCafe)

</div>

---

## 📡 What is this?

**CNT-Café Public Configs** is a free, continuously updated collection of working proxy configs for
**V2Ray / Xray**, **sing-box**, **Clash Meta** and any client that accepts a subscription link.
Every config in this repository has been **automatically tested and verified to work** within the last cycle —
no dead links, no "maybe it works" lists.

The list is refreshed automatically **7 times a day**, keeps a steady **200 working configs**,
and drops anything that stops working. Just point your client at the subscription URL below.

> 🌍 **Free internet access for everyone** — especially useful where access is restricted (Iran, China, Russia…).

---

## 📥 Subscription links

### 👉 Main subscription (recommended)

```
https://raw.githubusercontent.com/CNT-Cafe/Public-Configs/main/test-configs.txt
```

Copy the link, paste it into your client as a **subscription / remote config**, update, and connect.

### Direct file

```
https://github.com/CNT-Cafe/Public-Configs/blob/main/test-configs.txt
```

---

## 📱 Which client should I use?

| Platform | Client |
|---|---|
| **Android** | [V2rayNG](https://github.com/2dust/v2rayNG) · [NekoBox](https://github.com/MatsuriDayo/NekoBoxForAndroid) · [Hiddify](https://github.com/hiddify/hiddify-app) · [Streisand](https://apps.apple.com/app/streisand/id6450534064) |
| **iOS / iPadOS** | [Streisand](https://apps.apple.com/app/streisand/id6450534064) · [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118) · [Hiddify](https://apps.apple.com/app/hiddify-proxy-vpn/id6596777532) |
| **Windows** | [v2rayN](https://github.com/2dust/v2rayN) · [NekoRay](https://github.com/MatsuriDayo/nekoray) · [Hiddify](https://github.com/hiddify/hiddify-app) · [Clash Verge](https://github.com/clash-verge-rev/clash-verge-rev) |
| **macOS** | [V2Box](https://apps.apple.com/app/id6446814690) · [Hiddify](https://github.com/hiddify/hiddify-app) · [Clash Verge](https://github.com/clash-verge-rev/clash-verge-rev) |
| **Linux** | [NekoRay](https://github.com/MatsuriDayo/nekoray) · [Hiddify](https://github.com/hiddify/hiddify-app) |

**How to subscribe in V2rayNG:** `⋮` → *Subscription group settings* → `+` → paste the URL → save → tap *Update* (↻).

---

## ✅ Why are these configs better than other "free config" lists?

Most public lists are copy-paste dumps: most entries are dead, slow, or already blocked.
This repository is different — it is a **verified pipeline**, not a text dump:

- 🔬 **Every config is really tested.** Each one is started locally and must successfully
  fetch a live URL through its own tunnel before it is allowed into the list.
- 🛡️ **Iran-route gate.** Configs are additionally probed through an Iran vantage point,
  so published configs are usable **from Iran**, not just from a datacenter.
- 🔁 **Auto-healing.** Anything that fails a test is removed automatically. Failing configs
  do not linger.
- 🧭 **Real geo-location, by exit IP.** A config's country label is derived from its
  **actual exit IP** (GeoIP), never from its address/domain text. What you see is where you land.
- 🧱 **One-IP protection.** At most **5 configs per exit IP**, so a single dead server
  cannot flood the list — you get diversity, not twenty clones of the same node.
- 🧹 **Deduplicated** and normalized, with clean, sortable names:
  `☕️ CNTCafé1 • 🇩🇪 Germany`.

---

## 🌐 Supported protocols

| Protocol | Scheme |
|---|---|
| **VLESS** (+ Reality, XTLS-Vision) | `vless://` |
| **VMess** | `vmess://` |
| **Trojan** | `trojan://` |
| **Shadowsocks** | `ss://` |
| **Hysteria2** | `hysteria2://` / `hy2://` |

---

## 🗺️ What's inside a typical list?

A typical list is roughly **half European** and **a third North American**, with popular picks such as:

`🇺🇸 USA` · `🇳🇱 Netherlands` · `🇩🇪 Germany` · `🇫🇷 France` · `🇮🇹 Italy` · `🇬🇧 UK` · `🇭🇰 Hong Kong` · `🇯🇵 Japan` · `🇫🇮 Finland` …

The exact mix changes every cycle as nodes come and go.

---

## 🔧 How it works

```
 Sources (Telegram channels + public subscription URLs)
        │
        ▼
   Collect  ──►  Dedupe & normalize
        │
        ▼
   Test A  — every config must fetch a live page through its own tunnel
        │
        ▼
   GeoIP   — country label from the REAL exit IP (never from link text)
        │
        ▼
   Iran gate — probed through an Iran vantage point
        │
        ▼
   Publish — 200 working configs, max 5 per exit IP, refreshed 7×/day
```

Runs fully automatically on a schedule (**Asia/Tehran**): `00 · 02 · 04 · 08 · 12 · 16 · 20`.

---

## 📄 Repository files

| File | Description |
|---|---|
| `test-configs.txt` | The main subscription file — plain list of working `://` config links. |
| `✧ Public Configs` | Human-readable list with country flags and names. |
| `status.tsv` | Per-config table: protocol, country, last test result, latency, Iran status. |
| `flag_results.json` | Machine-readable results for the [@CNTCafe](https://t.me/CNTCafe) bot. |

---

## ❓ FAQ

<details>
<summary><b>Are these configs free?</b></summary>

Yes — completely free and open. They are collected from public sources and re-published.
</details>

<details>
<summary><b>How often is the list updated?</b></summary>

Automatically, **7 times a day** (00, 02, 04, 08, 12, 16, 20 Asia/Tehran). Your client
picks up fresh configs the next time you tap *Update*.
</details>

<details>
<summary><b>Why did a config stop working?</b></summary>

Remote servers go offline or get blocked all the time. Dead configs are removed on the
next cycle automatically — just update your subscription to get replacements.
</details>

<details>
<summary><b>Is it safe?</b></summary>

Configs are only tested for **connectivity**, not audited for privacy. Since these are
shared public nodes, do not send sensitive data through them. Use them for everyday browsing.
</details>

<details>
<summary><b>Do these work from Iran?</b></summary>

Yes — configs are specifically probed through an Iran vantage point, so the published list
is chosen to be usable from Iran, not only from other countries.
</details>

<details>
<summary><b>Can I use these on Clash / sing-box?</b></summary>

Yes. Paste the subscription URL into any client that supports remote subscriptions —
Clash Meta, sing-box, Hiddify, NekoBox, Streisand, Shadowrocket and others.
</details>

---

## 🔎 Keywords

free v2ray configs · free xray configs · free vless · free vmess · free trojan ·
free shadowsocks · free hysteria2 · v2ray subscription link · v2rayng config ·
neko box · hiddify · clash meta · sing-box · anti-censorship · Iran VPN ·
working proxy list · free proxy subscription · shadowsocks subscription

---

<div align="center">

**Made with ☕ by [CNT-Café](https://t.me/CNTCafe)**

⭐ Star this repo to support the project · 📡 [Join us on Telegram](https://t.me/CNTCafe)

</div>
