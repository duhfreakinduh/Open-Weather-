# AI / Contributor Guide

Keep the weather app lightweight and factual. AI may summarize retrieved forecast data, but it must not invent weather conditions, alerts, or confidence beyond the source data.

## Priorities
1. Source current conditions/forecast from an authoritative weather API before generating any summary.
2. AI summaries must be optional and grounded only in retrieved data.
3. Never put weather API keys or model/provider tokens directly in public client code.
4. Weather/network/AI failures must show a clear error or normal forecast fallback.
5. Do not generate or alter official severe-weather alerts with AI.
6. Keep location permission optional and provide manual location entry.
7. Preserve simple mobile usability and fast load time.
8. Document data sources, refresh behavior, and limitations.

## Before merging
- Test invalid/missing locations.
- Test denied geolocation permission.
- Test provider/network failure.
- Verify any AI summary matches the underlying numbers/conditions.
- Check mobile layout and console errors.
