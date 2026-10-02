# Trading Screen Rules — Detailed Specification

## 1. Allowed Instruments (Priority Order)

1. XAUUSD (Gold) — primary and preferred
2. EURUSD
3. GBPUSD
4. USDJPY
5. US30 (Dow)
6. NAS100 (Nasdaq)

Always prefer XAUUSD on M30 unless the user explicitly requests another pair.

## 2. Timeframe Rules

- Default and preferred: M30 (30-minute)
- Acceptable alternatives only when requested: H1, M15
- Never show random or unclear timeframes
- Timeframe selector must be readable when the UI is clear enough

## 3. Trade Structure Requirements

Every open trade shown on screen must include:

- Clear entry point (or current open position)
- Take Profit level visible
- Stop Loss level visible whenever possible
- Risk-Reward ratio approximately 1:3 or 1:4
- Current floating profit (positive in most cases)

## 4. Risk Management Limits

| Parameter        | Allowed Range                  | Forbidden                     |
|------------------|--------------------------------|-------------------------------|
| Lot size (Gold)  | 0.10 – 1.00 (typical 0.20–0.50)| 5+ lots, “all-in”             |
| Leverage shown   | 1:50 – 1:200                   | 1:500+, 1:1000+               |
| Open positions   | 1 main position preferred      | Many large simultaneous lots  |
| Risk appearance  | Controlled and professional    | Gambling / high-risk look     |

## 5. Indicator Rules

- Maximum two indicators on the chart
- Preferred combinations:
  - 50 EMA + RSI
  - 20 & 50 EMA
  - Bollinger Bands + RSI
  - MACD (alone or with one MA)
- Indicators must be correctly calculated and placed
- No random lines or decorative indicators

## 6. Platform Appearance Rules

### MetaTrader 5 Desktop
- Classic dark or light theme
- Visible elements when resolution allows: toolbar, chart, Market Watch, trade ticket or Toolbox
- Candles must look like real MT5 candlesticks

### MetaTrader 5 iPhone
- Realistic mobile layout (not desktop UI squeezed)
- Symbol, timeframe, and trade info readable
- Native iOS status bar optional but realistic if present

### TradingView
- Correct top toolbar, symbol, timeframe, and layout
- Clean chart with proper price scale
- No fake “AI-generated” chart look

## 7. Double-Check Procedure

For every image that contains a screen:

1. Run full Identity Lock checklist first.
2. Run full Trading Screen Accuracy checklist.
3. If any item fails:
   - Note the exact failure
   - Fix only that item (or the screen content)
   - Re-run the checklist for the fixed item
4. Only when both Identity and Screen pass → move to Physical Realism & Scene Logic.
5. Never restart the entire design because of one screen problem.

## 8. Prompt Guidance for Screens

When building the Variable Scene layer, include a clear screen description such as:

```
The main monitor shows MetaTrader 5 with XAUUSD M30 chart.
An open buy position is in profit.
Take Profit and Stop Loss lines are visible with approximately 1:3 risk-reward.
Lot size is 0.30. One or two standard indicators (50 EMA and RSI) are present.
Candles and prices look realistic and accurate.
```

## 9. Rejection Triggers (Screen Only)

Reject or fix the screen if:
- No clear trade is visible
- Timeframe is wrong or missing
- Lot size or leverage looks reckless
- Take Profit is missing on an open trade
- Candles look fake or randomly generated
- UI does not resemble real MT5 or TradingView
- More than two indicators clutter the chart
