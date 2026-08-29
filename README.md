# MeshCore Setup — Heltec ESP32 LoRa V4

🔒 Laatste security check: 2026-08-29 20:06 CEST

Documentatie voor het opzetten van een MeshCore mesh netwerk node op een Heltec ESP32 LoRa V4.

---

## Hardware

| Onderdeel | Details |
|-----------|---------|
| Board | Heltec ESP32 LoRa V4 |
| Chip | ESP32-S3 |
| Radio | SX1262 (LoRa) |
| Display | 0.96" OLED |
| Verbinding | USB-C |

---

## Stappen die NIET werkten

### ❌ CH343 USB driver (macOS)
- Driver gedownload van https://github.com/WCHSoftGroup/ch34xser_macos
- `.pkg` geïnstalleerd en reboot uitgevoerd
- macOS blokkeerde de driver stil (geen melding in Privacy & Beveiliging)
- Apparaat verscheen niet in `/dev/cu.*`
- **Conclusie:** CH343 driver werkt niet betrouwbaar op macOS 13+

---

## Firmware flashen

### ✅ Web flasher via Chrome (werkt wel)

1. Open **Google Chrome** (Safari werkt niet — geen WebSerial ondersteuning)
2. Ga naar https://flasher.meshcore.co.uk
3. Sluit Heltec aan via USB-C (gebruik een **datakabel**, niet alleen laadkabel)
4. Klik **Connect** en selecteer de USB poort
5. Kies model: **Heltec LoRa 32 V4**
6. Klik **Flash** en wacht tot klaar

> Geen driver nodig — Chrome's ingebouwde WebSerial API handelt dit af.

---

## Verbinding maken

1. Zet Heltec aan — witte LED knippert, display toont node info
2. Koppel apparaat via **Bluetooth** in je telefooninstellingen
3. Download de **MeshCore app**
4. Open de app en verbind met je node via Bluetooth

---

## Node configuratie

| Instelling | Waarde |
|------------|--------|
| Node naam | `NL-Ommeren-EdC` |
| Frequentie | 868 MHz (EU LoRa band) |
| Regio | `EU_868` |

### Naamgeving conventie
Zonder amateur radio callsign is er geen verplicht formaat. Aanbevolen: `LAND-PLAATS-NAAM` — bijv. `NL-Ommeren-EdC`.

---

## Testen

- Buiten testen voor maximaal bereik
- LoRa kan zonder obstakels meerdere kilometers bereiken
- Berichten versturen/ontvangen via de MeshCore app

---

## Links

- Web flasher: https://flasher.meshcore.co.uk
- CH343 driver (macOS, werkt niet goed): https://github.com/WCHSoftGroup/ch34xser_macos
- MeshCore: https://meshcore.co.uk
