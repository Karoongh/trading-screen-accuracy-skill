# trading-screen-accuracy

Reusable skill that forces every monitor or phone screen in generated images to show a realistic, accurate forex trade (primarily XAUUSD M30) with proper risk management, visible Take Profit / Stop Loss, and real MetaTrader 5 or TradingView UI.

Works together with the character-identity-lock skill.

## Install

Copy into your agent skills directory (e.g. `.grok/skills/trading-screen-accuracy/`).

## Key Rules

- Preferred: XAUUSD on M30
- Trade usually in profit
- Lot size and leverage realistic (not reckless)
- TP visible, SL preferred, RR ≈ 1:3 or 1:4
- Max two standard indicators
- UI must look like real MT5 (desktop/iPhone) or TradingView
- Fix only the failing item — never redesign the whole image

See SKILL.md and references/trading-screen-rules.md for full details.
