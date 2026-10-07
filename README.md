# Crypto Signal Lab · Trading Copilot v2

Een zelfstandige crypto trading-assistent die live publieke Bitvavo-marktdata combineert met technische analyse, patroonherkenning, multi-timeframe confluence, scenario's, risk management en paper trading.

## Nieuw in Copilot v2
- Beginner / Pro-modus
- Grote Trading Copilot-beslissing: LONG KANDIDAAT / SHORT KANDIDAAT / WACHT OP PULLBACK / NIET TRADEN
- Altijd een trigger, invalidatiepunt en belangrijkste risicofactor
- Automatische patroonherkenning:
  - EMA20 pullback
  - bullish breakout / bearish breakdown
  - hammer / shooting star
  - inside bar
  - bullish / bearish engulfing
  - double top / double bottom
  - Bollinger squeeze
  - bullish / bearish RSI-divergentie
- Patronen worden waar mogelijk ook als markers/levels op de chart gezet
- Automatische support- en resistancelevels
- Bull / Base / Bear scenario-engine met aparte scenario-scores en triggers
- 7-punts trade-checklist
- Strengere NO-TRADE-logica
- Opportunity Scanner voor meerdere EUR-markten op 1u + 4u
- Klik vanuit de scanner rechtstreeks een coin open
- Paper trading journal in localStorage
- Paper trades beginnen als PENDING en worden pas OPEN als de entryzone echt is geraakt
- Conservatieve afhandeling wanneer SL en TP in dezelfde candle vallen

## Reeds aanwezig
- Live Bitvavo REST + WebSocket candles
- Alle beschikbare EUR-markten
- 5m / 15m / 1u / 4u / 1D
- Candlesticks
- EMA20 / EMA50 / EMA200
- Bollinger Bands
- RSI14
- MACD 12/26/9
- ATR14
- ADX14
- Marktstructuur
- Multi-timeframe confluence 15m / 1u / 4u / 1D
- Entryzone, stop loss, TP1, TP2, TP3
- Risk/reward
- Positiecalculator op accountgrootte en risico per trade
- Responsive iPhone/tablet/desktop layout

## Beginner-modus
De nadruk ligt op gewone taal: wat gebeurt er, waarom is dat belangrijk, wat moet er eerst gebeuren vóór een trade, en wanneer is het idee ongeldig. De drukke RSI/MACD-subcharts worden verborgen.

## Pro-modus
Toont de onderliggende indicatorcharts en technische details, naast dezelfde scenario- en risk engine.

## Opportunity Scanner
De scanner haalt voor een geselecteerde set grotere EUR-markten 1u- en 4u-candles op en rangschikt setups op trend, momentum, ADX, volatiliteit en patroonconfluence. Een hoge scanner-score is geen winstkans of statistische probability; het is een interne kwaliteitsscore.

## Paper journal
Alles blijft lokaal in de browser via localStorage. Er is geen accountkoppeling of echte orderuitvoering. Een voorgestelde paper trade staat eerst PENDING. Hij wordt pas OPEN wanneer een volgende candle daadwerkelijk door de entryzone loopt. Daarna wordt SL of TP2 gevolgd zolang die markt opnieuw in de app wordt geladen.

## Starten
Open `index.html` in een moderne browser, of host het bestand op GitHub Pages.

## Belangrijk
Dit is een technische beslissingsondersteuner, geen winstmachine en geen persoonlijk beleggingsadvies. Marktdata en technische patronen kunnen abrupt ongeldig worden door nieuws, liquidaties, spreads, bugs, dataproblemen of regimewissels. Gebruik bij echt geld altijd een eigen risicolimiet en controleer belangrijk macro- en cryptonieuws.

## Externe onderdelen
- Publieke Bitvavo marktdata
- TradingView Lightweight Charts 5.2.1
