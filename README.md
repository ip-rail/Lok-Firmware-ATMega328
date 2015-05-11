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
<th> AVR Pin </th>
<th> Beschreibung </th>
<th> Anschluss an </th></tr>
<tr>
<td> 1</td>
<td> PD0</td>
<td> UART TXD</td>
<td> ESP8266 RXD </td></tr>
<tr>
<td> 2</td>
<td> PD1</td>
<td> UART RXD </td>
<td> ESP8266 TXD </td></tr>
<tr>
<td> 2</td>
<td> PC8</td>
<td> Reset </td>
<td> Taster </td></tr>
<tr>
<td> 3</td>
<td> GND  </td>
<td> GND Masse </td>
<td> GND Masse </td></tr>
<tr>
<td> 4</td>
<td> PD2 </td>
<td> t.b.d. </td>
<td> TLE Sens 1 </td></tr>
<tr>
<td> 5</td>
<td> PD3 </td>
<td> t.b.d. </td>
<td> TLE Sens 2 </td></tr>
</table>
