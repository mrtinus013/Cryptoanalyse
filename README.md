# Crypto Signal Lab

Een standalone live crypto-analysewebapp.

## Wat zit erin
- Live Bitvavo candles via publieke REST + WebSocket API
- BTC-EUR, ETH-EUR, SOL-EUR en automatisch alle beschikbare EUR-markten
- Timeframes: 5m, 15m, 1h, 4h, 1d
- Candlestick chart
- EMA 20 / 50 / 200
- Bollinger Bands
- RSI 14
- MACD 12/26/9
- ATR 14
- ADX 14
- Marktstructuur
- Multi-timeframe confluence (15m / 1h / 4h / 1d)
- LONG / SHORT / WACHTEN-classificatie
- Entryzone, Stop Loss, TP1/TP2/TP3 en R:R
- Risicocalculator op basis van accountgrootte en risico per trade
- Responsive layout voor iPhone, tablet en desktop

## Starten
Open `index.html` in een moderne browser.

Voor de betrouwbaarste werking kun je hem op GitHub Pages hosten:
1. Maak een nieuwe repository.
2. Upload `index.html`.
3. Settings -> Pages -> Deploy from branch.
4. Open de gegenereerde Pages-URL.

## Belangrijk
Deze app maakt technische scenario's op basis van marktdata. Het is geen garantie op winst en geen persoonlijk beleggingsadvies. Een technisch signaal kan abrupt ongeldig worden door nieuws, liquidaties, spreads of marktregimewissels.

## Externe onderdelen
- Bitvavo publieke marktdata
- TradingView Lightweight Charts

Technische chart-library is vastgezet op Lightweight Charts 5.2.1 voor reproduceerbaar gedrag.

## v1.1 – schaalfix
- Oude ENTRY/SL/TP-lijnen worden verwijderd vóór het laden van een nieuwe markt.
- Prijs- en tijdas worden na markt/timeframe-wissels expliciet opnieuw ge-autoscaled.
- Vertraagde API-responses van een eerder geselecteerde markt worden genegeerd.
- Live WebSocket-candles werken nu ook de chart en indicatorseries bij zonder automatisch je zoom te resetten.
