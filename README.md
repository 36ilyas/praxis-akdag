# Praxis Med. Dr. (Univ. Ist) Altan Akdag — Website

Statische Website für die Facharztpraxis für Psychiatrie und Psychotherapie,
Lindenstraße 260, 41063 Mönchengladbach.

Umgesetzt aus dem Design-Entwurf in [`entwurf1/`](entwurf1/) — reines HTML und CSS,
kein Build-Schritt, kein JavaScript (das Mobilmenü läuft über eine CSS-Checkbox).

## Struktur

```
index.html            Startseite (Hero, Praxis, Leistungen, Team, Ablauf, Hinweise, Kontakt)
impressum.html        Impressum — Pflichtangaben teilweise als Platzhalter
datenschutz.html      Datenschutzerklärung — Gerüst, muss juristisch geprüft werden
assets/css/style.css  Gesamtes Stylesheet
assets/img/           Bilder
entwurf1/             Ursprünglicher Design-Entwurf (Referenz, nicht Teil der Seite)
entwurf2/             Alternativer Design-Entwurf (nicht umgesetzt)
```

## Lokal ansehen

```bash
python -m http.server 5599
```

Dann http://localhost:5599 öffnen.

## Vor dem echten Livegang noch zu erledigen

- **Bilder austauschen:** Alle Fotos sind Platzhalter von [Unsplash](https://unsplash.com)
  (Unsplash-Lizenz, kommerziell nutzbar). Sie zeigen **nicht** die echten Praxisräume.
  Im Abschnitt „Das Team" gehört ein echtes Porträt von Dr. Akdag hin.
- **Impressum vervollständigen:** Kammer, KV, Aufsichtsbehörde, Berufshaftpflicht, E-Mail.
  Offene Stellen sind im Text farbig als `[… ergänzen]` markiert.
- **Datenschutzerklärung prüfen lassen** und um Hoster sowie tatsächlich eingesetzte
  Dienste ergänzen.
- **Google Maps & Google Fonts:** Beide laden aktuell direkt von Google und übertragen
  dabei die IP-Adresse der Besucher. DSGVO-sauberer wäre: Schriften lokal einbinden und
  die Karte erst nach Einwilligung nachladen (Zwei-Klick-Lösung).
- **Bewertungszahl prüfen:** „5,0 aus 316 Bewertungen" stammt aus dem Entwurf und sollte
  mit dem aktuellen Stand des Google-Profils abgeglichen werden.

## Veröffentlichung

Die Seite wird über GitHub Pages aus dem `main`-Branch (Wurzelverzeichnis) ausgeliefert.
