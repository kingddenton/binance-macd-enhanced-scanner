# Project Brief — Binance MACD Enhanced Scanner

**Last documented:** 16 November 2026  
**Repository:** [kingddenton/binance-macd-enhanced-scanner](https://github.com/kingddenton/binance-macd-enhanced-scanner)  
**Selected working page:** [Candle Monitor_2](https://kingddenton.github.io/binance-macd-enhanced-scanner/test-preview/candle-monitor-2.html)

## 1. Project purpose

A browser-based Binance USDⓈ-M USDT perpetual-futures market scanner. It is a monitoring and alerting tool; it does not place trades. The current selected copy is to be preserved as the stable working version.

## 2. Authoritative baseline

- **Working source:** `test-preview/candle-monitor-2.html`
- **Source blob SHA at backup:** `5d9e72ad87b2aa738ab4e7f2ef4919ec4e5df151`
- **Baseline commit immediately before backup:** `6983df187871f26645fa666b09c5ecbd04e3e385`
- **Exact backup copy:** `backups/candle-monitor-2-stable-2026-11-16.html`
- **Backup creation commit:** `c56e777e1fc787a5ba16647f959ec3420ae42c66`

The backup is an exact copy of the selected working HTML file at the source SHA above. It is retained separately; do not edit the backup during normal development.

## 3. Current alert-card presentation

The Bullish Cross and Bearish Reversal alert cards share the same layout:
- Coin symbol aligned left.
- Candle count (for example, `2/5`) centred.
- 24-hour price change aligned right.
- Card text is set to 16px, with the candle count bolded to match the other values.
- Positive 24-hour changes are green; negative changes are red.
- Timeframe headings (1M, 3M, 5M and 15M) are set to 16px.
- Bullish and bearish groups remain vertically stacked, with bullish above bearish.

These are presentation choices; do not change alert eligibility, candle counting, signal detection or timing as part of a visual-only request.

## 4. Timeframes and alert behavior documented in the selected copy

- Special Bullish Cross and Bearish Reversal displays include 1m, 3m, 5m and 15m columns.
- The card display shows up to five active entries per direction, subject to the existing candle-limit and expiry logic in the source.
- Directional 24-hour qualification was previously implemented: bullish candidates require positive 24-hour change; bearish candidates require negative 24-hour change.
- Existing live/closed-candle detection mode, confirmations, thresholds, volume checks, sounds and other scanner logic must be preserved unless a change is explicitly requested.

This brief records the known design and prior agreed behavior; it is not a fresh mathematical or end-to-end audit of every scanner subsystem.

## 5. Working rules — important

1. **Use only** `test-preview/candle-monitor-2.html` as the active working file unless the user explicitly selects another file.
2. Before every edit, fetch the latest file and its current SHA. Make only the narrowly requested change.
3. Preserve all unrelated UI, scanner logic, settings, alert rules and API behavior.
4. Do not rebuild, switch versions, restore another backup, or refactor without explicit approval.
5. After editing, fetch the file again and verify the exact requested changes and resulting SHA.
6. Distinguish a committed GitHub source update from a published GitHub Pages update. Do not claim the live page has changed until deployment is confirmed.
7. The scanner uses public Binance market data; do not introduce an API-key requirement.
8. Keep performance and stability in mind. Do not add unnecessary API calls, diagnostics, polling or extra calculations without approval.

## 6. Change control

The user has explicitly chosen to keep this current copy as the stable working version. No further changes are authorized by this brief alone. Make future modifications only in response to a clear user request, and keep this brief and the dated backup as reference points.

## 7. Current reference links

- Working page: https://kingddenton.github.io/binance-macd-enhanced-scanner/test-preview/candle-monitor-2.html
- Working source: https://github.com/kingddenton/binance-macd-enhanced-scanner/blob/main/test-preview/candle-monitor-2.html
- Backup source: https://github.com/kingddenton/binance-macd-enhanced-scanner/blob/main/backups/candle-monitor-2-stable-2026-11-16.html
