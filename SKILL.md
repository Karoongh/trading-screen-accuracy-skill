---
name: trading-screen-accuracy
description: Enforce realistic and accurate trading screen content (MetaTrader 5 or TradingView) in all generated images that show monitors or phones. Use when creating, reviewing or fixing images of FX-TRADER-01 or any character that displays forex charts, especially XAUUSD and major pairs. Triggers on trading screen, monitor chart, MT5, MetaTrader, TradingView, XAUUSD, candle, take profit, stop loss, lot size, leverage, or realistic trade result.
---

# Trading Screen Accuracy

## Overview

Every monitor or phone screen that appears in a generated image must display a realistic, accurate, and professionally plausible forex trade. The primary focus is XAUUSD (Gold) on the 30-minute timeframe, with support for other major pairs. Screens must look like real MetaTrader 5 (desktop or iPhone) or TradingView.

This skill works together with character-identity-lock. Identity is checked first. Trading screen content is checked second. Only the failing part is fixed — never redesign the entire image.

## Core Principles (Mandatory)

1. Screens are never decorative. Every visible chart must show a real-looking trade.
2. Preferred pair: XAUUSD on M30 timeframe.
3. Allowed pairs (in order of priority): XAUUSD, EURUSD, GBPUSD, USDJPY, US30, NAS100.
4. Trade must usually be in profit.
5. Lot size and leverage must be realistic and not reckless.
6. Take Profit must be visible. Stop Loss should be visible when possible.
7. Risk-Reward ratio target: 1:3 or 1:4.
8. Candles, prices, and indicators must look accurate and consistent with real market behavior.
9. UI must resemble real MetaTrader 5 (Windows or iPhone) or TradingView.
10. If any screen rule fails → fix only that problem. Do not regenerate identity or the whole scene.

## Required Screen Content Checklist

Before approving any image that contains a monitor or phone:

### A. Platform and Timeframe
- [ ] Platform is clearly MT5 desktop, MT5 iPhone, or TradingView
- [ ] Timeframe is M30 (preferred) or clearly stated
- [ ] Pair is one of the allowed pairs (XAUUSD preferred)

### B. Trade Reality
- [ ] Candles look realistic (proper body/wick ratios, no random noise)
- [ ] Current price is consistent with recent candles
- [ ] Trade is in profit (or very close and still valid)
- [ ] Entry, Take Profit and preferably Stop Loss are visible
- [ ] Risk-Reward is approximately 1:3 or 1:4

### C. Risk Management
- [ ] Lot size is logical (0.10 – 1.00 for gold on standard account, never extreme)
- [ ] Leverage is reasonable (not 1:1000 or higher shown as normal)
- [ ] Not multiple oversized positions open at once
- [ ] No all-in or gambling appearance

### D. Indicators
- [ ] Maximum one or two well-known indicators (Moving Average, RSI, MACD, Bollinger Bands)
- [ ] Indicators are correctly placed and do not clutter the chart

### E. UI Fidelity
- [ ] MT5 look: toolbar, market watch, navigator, chart window, trade tab if visible
- [ ] iPhone MT5: realistic mobile layout, not desktop stretched
- [ ] TradingView: correct toolbar, timeframe selector, symbol, and layout
- [ ] No obviously fake or generic AI chart appearance

## Fix Policy (Critical)

When a problem is found:

1. Identify the exact failing item (e.g. lot size too large, no Take Profit visible, wrong timeframe).
2. Regenerate or edit only the screen content or the specific issue.
3. Do not change the character identity, body, clothing, or overall composition unless they are also failing their own checklist.
4. Re-check the fixed item and the full screen checklist again.
5. Only after the screen passes, proceed to final approval.

## Integration with Character Identity Lock

Order of checks for every image:

1. Identity Lock (face, age, hair, beard, body) — from character-identity-lock
2. Trading Screen Accuracy (this skill)
3. Physical Realism and Scene Logic (hands, gaze, props, shadows)

Fail any layer → reject or fix only that layer.

## Preferred Trade Example (XAUUSD M30)

A good default trade description for prompts:

- Symbol: XAUUSD
- Timeframe: M30
- Direction: Buy or Sell (in profit)
- Lot size: 0.20 – 0.50
- Risk-Reward: approximately 1:3 or 1:4
- Visible Take Profit line
- Visible Stop Loss line (preferred)
- One or two indicators: e.g. 50 EMA + RSI
- Platform: MetaTrader 5 desktop or iPhone, or TradingView

## Negative Constraints for Screens

Never allow:
- Random or decorative charts with no clear trade
- Extreme lot sizes or leverage that look reckless
- Multiple large positions that imply gambling
- Missing Take Profit when a trade is open
- Obviously fake candles or prices
- Desktop UI stretched onto a phone or vice versa
- Cluttered charts with more than two indicators

## When to Activate

Activate this skill automatically whenever:
- A monitor, laptop screen, or phone is visible in the image
- The scene is Trading / Technical
- The user mentions XAUUSD, gold, charts, MT5, TradingView, or trade results
