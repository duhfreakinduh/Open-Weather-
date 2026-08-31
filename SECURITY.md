# Security Policy

## Reporting a vulnerability
Do not post secrets, private URLs, precise location data, exploit details, or sensitive logs in a public issue. Use GitHub private vulnerability reporting if enabled; otherwise open only a minimal issue until a private channel is established.

## Security expectations
- Never commit weather API keys or model/provider tokens.
- Treat precise location as private user data.
- Do not let AI invent or modify official severe-weather alerts.
- Ground generated summaries in retrieved forecast data only.
- Bound network/model calls with timeouts and safe fallbacks.
- Review third-party API/CDN changes before release.
