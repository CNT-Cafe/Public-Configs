<div align="center">

# ☕ CNTCafé Public Configs

**Free, automatically-tested V2Ray / Xray proxy configs — refreshed 6 times a day.**
VLESS · VMess · Trojan · Shadowsocks · Hysteria2 — for V2rayNG, Hiddify, NekoBox, v2rayN, V2Box, Happ, Streisand, Clash Meta & more.

[![Live](https://img.shields.io/badge/status-live%20%26%20auto--updated-brightgreen)](https://github.com/CNT-Cafe/Public-Configs)
[![Configs](https://img.shields.io/badge/configs-200%20working-blue)](https://github.com/CNT-Cafe/Public-Configs)
[![Tested](https://img.shields.io/badge/tested-from%20a%20real%20Iran%20IP-red)](https://github.com/CNT-Cafe/Public-Configs)
[![Protocols](https://img.shields.io/badge/protocols-VLESS%20%C2%B7%20VMess%20%C2%B7%20Trojan%20%C2%B7%20SS%20%C2%B7%20Hysteria2-orange)](https://github.com/CNT-Cafe/Public-Configs)

[📥 **Subscribe**](#-subscription-link) · [🇮🇷 نسخهٔ فارسی](README.fa.md) · [❓ FAQ](#-faq) · [📡 Telegram](https://t.me/CNTCafe)

</div>

---

## 📡 What is this?

**CNT-Café Public Configs** is a free, continuously updated collection of **working** proxy configs
for **V2Ray / Xray**, **sing-box**, **Clash Meta** and any client that accepts a subscription link.
Every config here has been **automatically tested** within the last cycle — no dead links, no
"maybe it works" lists.

The list is refreshed automatically **6 times a day**, keeps a steady **200 working configs**, and
drops anything that stops working. Just point your client at the subscription URL below.

> 🌍 Free internet access for everyone — especially where access is restricted.

---

## 📥 Subscription link

### 👉 Main subscription (recommended)

```
https://raw.githubusercontent.com/CNT-Cafe/Public-Configs/main/%E2%9C%A7%20Public%20Configs
```

> If your app cannot open a link containing a space or a `✧`, use the percent-encoded URL above
> (it is the very same file).

Copy the link, paste it into the client as a **subscription**, update, and connect.

---

## 🔬 The three things that make this list different

### 1. Tested from a **real Iranian IP — not a datacenter**

Most "free config" lists test from a datacenter in Europe. That proves nothing about whether a
config works **from inside Iran**. This project probes every config through a **genuine Iranian
residential connection** — a rotating SIM that covers the real Iranian mobile networks:

> 🇮🇷 **Rightel · APTEL · Irancell**

A config is published **only if it actually connects from Iran** — not from a datacenter, not from
a VPN, not from a "close enough" location. That is why what you see here tends to actually work
when you import it.

### 2. **Security filter** — weak, unencrypted configs are refused

A huge share of configs floating around are `ws + no TLS` or `tcp raw`: no encryption, no
integrity, nothing. **This list refuses to publish them at the source:**

| Rejected at collection | Why |
|---|---|
| `vless` with `security=none` (ws/tcp raw, no TLS) | no encryption |
| `trojan` with `security=none` | no encryption |
| `hysteria2` with `insecure=1` | certificate validation disabled |

Only configs that carry real transport security — **Reality, TLS, XTLS-Vision, ML-KEM** — make it
into the list. Security is a first-class requirement here, not an afterthought.

### 3. **No more copy-paste spam — we already deduplicated for you**

Here is the daily pain this project removes. On Telegram, dozens of channels re-post **the same
configs**, only renamed. A user joins ten groups, tests ten configs, and finds out that **eight of
them were literally the same node with different names.** Hours of copying, pasting, testing and
guessing — for one working connection.

**This subscription does all of that automatically:**

- 🔁 **Deduplicated** — the same endpoint cannot appear twice under two names. What you get is
  genuinely *different* servers, not ten aliases of one.
- ✅ **Pre-tested** — every entry already passed a real connection test before you saw it.
- 🌍 **Pre-labelled** — a config is labelled by its **real exit IP** (GeoIP), never by the text
  in its link. What you see is where you actually land.
- 🧱 **One-IP cap** — at most **5 configs per exit IP**, so one dead server cannot flood the list.

**You no longer have to join dozens of Telegram channels to find a free config.** Import this
subscription once, and you are done.

---

## 📱 Works in every popular client

Including the apps most used inside Iran:

`V2rayNG` · `v2rayN` · `Hiddify` · `NekoBox` · `NekoRay` · `Streisand` · `V2Box` · `Shadowrocket` ·
`Clash Meta` · `Happ` · `Incy` · `ZedSecure` · `PattNG` · `NPV Tunnel`

| Platform | Clients |
|---|---|
| **Android** | V2rayNG · NekoBox · Hiddify · **Incy** · **PattNG** · **NPV Tunnel** · **Happ** |
| **iOS** | Streisand · Shadowrocket · **V2Box** · **ZedSecure** · **Happ** |
| **Windows** | v2rayN · NekoRay · Hiddify · Clash Verge |
| **macOS** | V2Box · Hiddify · Clash Verge |
| **Linux** | NekoRay · Hiddify |

**V2rayNG:** `⋮` → *Subscription group settings* → `+` → paste the URL → save → tap *Update* (↻).

---

## 🌐 Supported protocols

| Protocol | Scheme |
|---|---|
| **VLESS** (+ Reality, XTLS-Vision, ML-KEM) | `vless://` |
| **VMess** | `vmess://` |
| **Trojan** | `trojan://` |
| **Shadowsocks** | `ss://` |
| **Hysteria2** | `hysteria2://` / `hy2://` |

---

## 🗺️ What's inside?

A typical list is roughly **half European** and **a third North American**, with popular picks such as:

`🇺🇸 USA` · `🇳🇱 Netherlands` · `🇩🇪 Germany` · `🇫🇷 France` · `🇮🇹 Italy` · `🇬🇧 UK` · `🇭🇰 Hong Kong` · `🇯🇵 Japan` · `🇫🇮 Finland` …

The exact mix changes every cycle as nodes come and go.

---

## 🔧 How it works

```
 Sources (Telegram channels + public subscription URLs)
        │
        ▼
   Collect  ──►  Dedupe & normalize  ──►  Security filter (no plaintext configs)
        │
        ▼
   Test A  — every config must open a real page through its own tunnel
        │
        ▼
   GeoIP   — country label from the REAL exit IP (never from link text)
        │
        ▼
   Iran gate (HARD) — must connect from a real Iranian IP (Rightel / APTEL / Irancell)
        │               a config that fails here is NOT published.
        ▼
   Publish — 200 working configs, max 5 per exit IP, refreshed 6×/day
```

Runs fully automatically (**Asia/Tehran**): `00 · 03 · 08 · 12 · 16 · 20`.
The **Iran gate runs at 16, 20, 00 and 03** — a **hard gate**: a config must pass both
Test A **and** the Iran test to be published. (The 08 and 12 cycles are Test A only.)

---

## 📄 Repository files

| File | Description |
|---|---|
| `✧ Public Configs` | **The subscription file** — plain list of working config links with country labels. |
| `status.tsv` | Per-config table: protocol, country, last test result, latency, Iran status. |
| `README.md` / `README.fa.md` | This documentation (English / فارسی). |

---

## ❓ FAQ

<details>
<summary><b>Are these configs free?</b></summary>

Yes — completely free. They are collected from public sources, tested, and re-published.
</details>

<details>
<summary><b>How often is the list updated?</b></summary>

Automatically **6 times a day** (00, 03, 08, 12, 16, 20 Asia/Tehran). Your client picks up fresh
configs the next time you tap *Update*.
</details>

<details>
<summary><b>Are the configs really tested from Iran?</b></summary>

Yes. Every config is probed through a **real Iranian residential connection** on the rotating SIM
(Rightel, APTEL, Irancell). The Iran test is a **hard gate**: a config that cannot connect from
Iran is not published.
</details>

<details>
<summary><b>Why are so many configs missing compared to other lists?</b></summary>

Because most of them **do not work**, are **unencrypted**, or are **duplicates of each other**.
This list keeps only what passed a real connection test and carries real transport security.
Quality over quantity.
</details>

<details>
<summary><b>Are the same configs renamed and re-posted?</b></summary>

No. Duplicate endpoints are detected and collapsed, so the same server does not appear under
several names. This is one of the main problems this project solves.
</details>

<details>
<summary><b>Is it safe?</b></summary>

Configs are tested for **connectivity** and filtered for **transport security**, but they are shared
public nodes — do not send sensitive data through them. Use them for everyday browsing.
</details>

---

## 🔎 Keywords

free v2ray configs · free xray configs · free vless · free vmess · free trojan · free shadowsocks ·
free hysteria2 · v2ray subscription link · v2rayng config · tested from Iran · Iran vpn · Rightel ·
Irancell · APTEL · anti-censorship · working proxy list · free proxy subscription · clash meta ·
sing-box · neko box · hiddify · incy · zedsecure · PattNG · V2Box · Happ · NPV Tunnel

---

<div align="center">

**Made with ☕ by [CNT-Café](https://t.me/CNTCafe)**

⭐ Star this repo to support the project · 📡 [Join us on Telegram](https://t.me/CNTCafe)

</div>
