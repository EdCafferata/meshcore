# MeshCore Repeater — Buiten Off-Grid Setup

Documentatie voor het plaatsen van een off-grid MeshCore repeater op een buitenlocatie (bijv. dak Kroonheuvel 9, Ommeren).

---

## Doel

Bereik vergroten tussen nodes die te ver van elkaar staan voor directe LoRa verbinding (>15-20 km). Een repeater op een hoge locatie overbrugt dit door berichten door te sturen via de mesh.

---

## Complete kit (aanbevolen)

**[MeshCore/Meshtastic Solar Outdoor Repeater — Etsy](https://www.etsy.com/listing/4310813646/meshcore-or-meshtatstic-solar-outdoor)**

| Onderdeel | Details |
|-----------|---------|
| Board | Heltec LoRa 32 V4 (+28 dBm) |
| Antenne | +5.5 dBi glasvezel, 868 MHz EU |
| Zonnepaneel | 25W met MPPT lader |
| Behuizing | IP67 waterdicht |
| Montage | Beuvel voor 38mm of 50mm TV mast |
| Firmware | Flash MeshCore repeater firmware |

Alles zit in één kit — alleen MeshCore firmware nog flashen via [flasher.meshcore.co.uk](https://flasher.meshcore.co.uk).

---

## Beste losse antenne

**[Paradar 868MHz 8.5 dBi outdoor antenne](https://pileupdx.com/product/paradar-868mhz-outdoor-antenna-8-5-dbi/)**

- 8.5 dBi gain — maximaal bereik
- Glasvezel radome met koper/messing binnenwerk
- Windbestendig tot 215 km/u
- Geschikt voor permanente buitenmontage

---

## Locatie

| Instelling | Waarde |
|------------|--------|
| Locatie | Dak Kroonheuvel 9, Ommeren |
| Hoogte | Verhoogd punt, vrij zicht Betuwe |
| Voeding | Off-grid zonnepaneel |
| Verwacht bereik | Tiel, Kesteren, Dodewaard en omgeving |

---

## Frequentie

Zorg dat de repeater op dezelfde frequentie staat als het netwerk:

| Instelling | Waarde |
|------------|--------|
| Regio | EU/UK (NARROW) |
| Frequentie | 869.618 MHz |
| Band | 62.5 kHz |
| Spreading Factor | SF8 |
| Codering | 4/8 |
| Vermogen | 28 dBm |

---

## Links

- Web flasher: https://flasher.meshcore.co.uk
- Complete kit: https://www.etsy.com/listing/4310813646/meshcore-or-meshtatstic-solar-outdoor
- Taoglas Barracuda 868MHz 8dBi antenne: https://www.taoglas.com/product/barracuda-omb-868-08f21-868mhz-8dbi-omni-directional-outdoor-antenna/
- ODL Store 8dBi alternatief: https://odlstore.com/lora-iot-modules-and-kits/602-lora-antenna-433mhz-470mhz-868mhz-915mhz-8dbi-fiber-glass-antenna-with-n-female-connector.html
