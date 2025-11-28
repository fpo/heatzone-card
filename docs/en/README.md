# HeatZone Card's

[![EN](https://img.shields.io/badge/EN-English-blue)](https://github.com/fpo/heatzone-card/blob/main/docs/en/README.md) [![DE](https://img.shields.io/badge/DE-Deutsch-red)](https://github.com/fpo/heatzone-card/blob/main/docs/de/README.md)

Custom Lovelace maps for controlling/displaying heating zones in Home Assistant.
Only functional in conjunction with the HeatZone integration.

## Installation über HACS

![Warning](/assets/warning-red-warning-en.svg)

This is necessary, because the heatzone card opens the heatzone profile card as a popup window.
The dual installation may seem inconvenient at first, but it has the advantage that
the cards can also be updated separately.

**1. Installation heatzone-card:** 

[![Add to HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=fpo&repository=heatzone-card&category=plugin)

Or alternatively

1. In HACS → `Integrations` → click the three dots in the upper right corner → **Custom Repository**.
2. URL https://github.com/fpo/heatzone-card Category: **Dashboard**.
3. Then, in HACS, search for **HeatZone Card** under `Frontend` and install it.
4. HACS will place the file in `www/community/heatzone-card/heatzone-card.js`.

The resource is usually added automatically by HACS. If not, add it manually:

```yaml
resources:
  - url: /hacsfiles/heatzone-card/heatzone-card.js
    type: module
```

**2. Installation heatzone-profile-card:** 

[![Add to HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=fpo&repository=heatzone-profile-card&category=plugin)

Or alternatively

1. In HACS → `Integrations` → click the three dots in the upper right corner → **Custom Repository**.
2. URL https://github.com/fpo/heatzone-profile-card Category: **Dashboard**.
3. Then, in HACS, search for **HeatZone Card** under `Frontend` and install it.
4. HACS will place the file in `www/community/heatzone-card/heatzone-profile-card.js`.

The resource is usually added automatically by HACS. If not, add it manually:

```yaml
resources:
  - url: /hacsfiles/heatzone-card/heatzone-profile-card.js
    type: module
```
