# Swing Scanner

Forex swing trade scanner — 28 pairs, H4 + H1, Twelve Data API.

## Deploy to Vercel

```bash
cd swing-scanner
vercel --prod
```

No environment variables needed — API key is entered in the UI and saved to localStorage.

## What it does

- Scans 28 pairs on H4 for swing moves 300+ pips
- Checks MA 9/20 alignment and MACD direction
- Detects H4 consolidation (false start filter)
- Checks H1 for consolidation breakout signal inside the H4 swing
- Calculates stop distance from previous candle high/low
- Signals: Ready / Consolidating / Watch / No setup
