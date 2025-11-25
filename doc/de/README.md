# HeatZone Card's

[![DE](https://img.shields.io/badge/DE-Deutsch-red)](/doc/de/README.md) [![EN](https://img.shields.io/badge/EN-English-blue)](/doc/en/README.md)

Custom Lovelace-Karten für die Steuerung / Darstellung von Heizungszonen in Home Assistant.
Nur in Verbindung mit der HeatZone Integration sinnvoll funktionsfähig.

## Installation über HACS

![Warning](/assets/warning-red-warning-de.svg)

Das ist nötig da die heatzone-card als Popup-Window die heatzone-profile-card aufruft.
Die zweifache Installation scheint erst einmal unkomfortabel, hat aber den Vorteil,
das die Karten auch separat aktualisiert werden können.

**1. Installation heatzone-card:** 

[![Add to HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=fpo&repository=heatzone-card&category=plugin)

Oder Alternativ

1. In HACS → `Integrationen` → oben rechts auf die drei Punkte → **Benutzerdefiniertes Repository**.
2. URL https://github.com/fpo/heatzone-card Kategorie: **Dashboard**.
3. Danach in HACS unter `Frontend` nach **HeatZone Card** suchen und installieren.
4. HACS legt die Datei unter `www/community/heatzone-card/heatzone-card.js` ab.

Die Ressource wird in der Regel automatisch von HACS hinzugefügt. Falls nicht, manuell:

```yaml
resources:
  - url: /hacsfiles/heatzone-card/heatzone-card.js
    type: module
```

**2. Installation heatzone-profile-card:** 

[![Add to HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=fpo&repository=heatzone-profile-card&category=plugin)

Oder Alternativ

1. In HACS → `Integrationen` → oben rechts auf die drei Punkte → **Benutzerdefiniertes Repository**.
2. URL https://github.com/fpo/heatzone-profile-card Kategorie: **Dashboard**.
3. Danach in HACS unter `Frontend` nach **HeatZone Profile Card** suchen und installieren.
4. HACS legt die Datei unter `www/community/heatzone-profile-card/heatzone-profile-card.js` ab.

Die Ressource wird in der Regel automatisch von HACS hinzugefügt. Falls nicht, manuell:

```yaml
resources:
  - url: /hacsfiles/heatzone-card/heatzone-profile-card.js
    type: module
```