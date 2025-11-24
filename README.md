# NVDIO

A lightweight web page that mirrors the provided Access/VBA workflow: enter one or more ticker symbols and fetch their current price plus 52-week high/low information from Yahoo Finance's chart API.

## Running locally

Because everything is client-side, you can open `index.html` directly in a browser or serve it from any static host.

```bash
# Example using Python
python -m http.server 8000
# then visit http://localhost:8000
```

## Features
- Comma-separated ticker input and progress messaging
- Client-side fetch against `query1.finance.yahoo.com`
- 52-week low/high calculation with percentage distances from the current price
- Inline error rows for tickers that fail to return data
