# Crypto Signal Lab · Unified Trading Copilot v4

## Belangrijkste wijziging
De app geeft nu **één gecombineerd advies per tradingpair**.

Het hoofdadvies verandert niet meer omdat je een andere grafiekweergave opent.

### Weging
- 15m: timing (10%)
- 1u: setup en entry (30%)
- 4u: hoofdtrend (40%)
- 1D: bredere context (20%)

Een LONG of SHORT wordt alleen afgegeven wanneer de gezamenlijke score sterk genoeg is en de belangrijke timeframes niet hard tegen elkaar ingaan. Anders staat er **NIET HANDELEN**.

## Interface
- Tradingpair kiezen bovenaan
- Eén groot gecombineerd advies: LONG / SHORT / NIET HANDELEN
- Eén confidence-score
- Eén entryzone, stop loss en TP-plan
- Trigger, invalidatie en belangrijkste risico
- Chart-timeframe is verplaatst naar de grafiek en is alleen een weergavekeuze
- Verdiepende timeframe-data blijft beschikbaar, maar zit uit de hoofdflow
- Opportunity Scanner gebruikt nu dezelfde 4-timeframe combinatie per coin

## Data
Publieke Bitvavo REST + WebSocket marktdata.
