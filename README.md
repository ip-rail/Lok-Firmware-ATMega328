# Lok-Firmware-ATMega328

Firmware for ATMega328p loco controller with serial WIFI module (ESP8266/Raspberry Pi/..) to control G-scale train engines

## Funktionalität

- [x] Ansteuerung H-Brücke PHB01
- [x] Kommunikation über serielles WLAN Modul
- [ ] i2c (Ansteuerung LED Controller PCA9622 Adapterboard PLED01)
- [ ] Servo Ansteuerung
- [ ] Motor Regelung

### Erweiterte Funktionalitäten
- [ ] Hall Sensor zur Motor Regelung
- [ ] Spannungs Überwachung
- [ ] Temperatur Überwachung
- [ ] Abstands Sensor
- [ ] RFID Schnittstelle
- [ ] SUSI Schnittstelle
- [ ] DCC Empfang

## Pin-Belegung 

Beta-Version:
<table class="wikitable sortable">

<tr>
<th> No </th>
<th> AVR Pin </th></tr>
<th> Beschreibung </th></tr></tr>
<tr>
<td> 1</td>
<th> PD0</th></tr>
<td> UART TXD: Anbindung an ESP8266 RXD </th></tr></tr>
<tr>
<td> PD1</td>
<td> UART RXD: Anbindung an ESP8266 TXD
</th></tr></tr>
<tr>
<td> PC8</td>
<td> Reset
</th></tr></tr>
<tr>
<td> GND  </td>
<td> GND Masse
</th></tr></tr>
<tr>
<td> PD2 </td>
<td> TLE Sens 1
</th></tr></tr>
<tr>
<td> PD3 </td>
<td> TLE Sens 2
</th></tr></tr></table>
