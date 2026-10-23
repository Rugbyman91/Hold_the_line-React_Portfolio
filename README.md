# Hold the Line

Een autobattler in React: kies je facties, bouw een team in de shop
en overleef 20 golven aan automatische gevechten.

Speel het hier: https://rugbyman91.itch.io/hold-the-line

## Gameplay
- Kies 1 tot 5 facties om je run mee te starten
- Shop met 3 willekeurige eenheden, gefilterd op factie en tier;
  eerste reroll gratis, daarna 1 goud
- Eenheden kopen, verplaatsen en verkopen via drag-and-drop
  tussen shop, team (8 plaatsen) en bench (5 plaatsen)
- Drie gelijke eenheden worden samengevoegd tot een geëvolueerde versie
- Automatisch turn based gevecht: frontrow wordt eerst aangevallen,
  daarna de backrow; snelheid instelbaar op 1x, 2x of 3x
- 20 golven met goudbeloning na elke gewonnen golf

## Technologie
React, Vite, React Router, CSS-animaties

## Hoe starten
npm install
npm run dev

## Technische keuzes
- Gedeelde spelstate (goud, golf, team, bench) via React Router's
  outlet context
- Gevechtslus als async functie met een annuleringsvlag, zodat
  een gevecht netjes stopt als de component verdwijnt
- Data van eenheden en golven staat los van de componenten
- Animaties via CSS-klassen die in de lus worden aan- en uitgezet

## Mogelijke uitbreidingen
- Skills
- Items (equip en use)
- Neutral faction die standaard als factie meegeselecteerd wordt
