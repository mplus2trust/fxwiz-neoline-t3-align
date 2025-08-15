# fxwiz-neoline-t3-align
Public source code release for FXWIZ NeoLine–T3 Align (Invite-Only on TradingView). Provided to comply with MPL-2.0; includes NOTICE and full source.

# FXWIZ NeoLine–T3 Align – Public Source Release

This repository contains the **full source code** for the FXWIZ NeoLine–T3 Align
indicator, as required under the **Mozilla Public License 2.0 (MPL-2.0)**.

## ✨ What it does
- **NeoLine (BB+ATR) reversal engine**
- **RSI-adaptive T3** alignment filter
- **Single-bar BG highlight** on alignment events
- **MTF cross table** (1/5/15/30/60m, no lookahead)
- **Alerts** for trend flip & align events

## 🔧 How it works (brief)
- NeoLine detects reversal using Bollinger Bands and ATR shift.
- An RSI-driven adaptive T3 smooths price for alignment.
- When trade mode is set (buy/sell) and NeoLine crosses the T3 accordingly,
  a one-bar background highlight appears.
- MTF table summarizes cross states per timeframe.

## ⚙️ Inputs (defaults)
- NeoLine: BB(21, dev 1.0), ATR(5), ATR filter ON
- T3: RSI(14) → adaptive length [5..50], factor 0.7
- BG: Align-only highlight, instant-on at signal = ON

## 🔔 Alerts
- `NeoLine Trend BUY / SELL`
- `ALIGN BUY / SELL`

## 📄 License
This code is licensed under the [Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/).

## 📂 Files
- **FXWIZ_NeoLine_T3_Align.pine** — Full Pine Script® source
- **NOTICE** — Credits & acknowledgements
- **LICENSE** — MPL-2.0 text

## 📈 TradingView
Distributed as **Invite-Only** to authorized FXWIZ members.

## 📝 Changelog
**v1.0 (2025-08-08)** — Initial release:
NeoLine(ATR/BB) + RSI-adaptive T3 alignment, single-bar BG highlights,
MTF cross table, alerts.
