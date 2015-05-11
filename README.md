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
<td> 3</td>
<td> PC8</td>
<td> Reset </td>
<td> Taster </td></tr>
<tr>
<td> 4</td>
<td> GND  </td>
<td> GND Masse </td>
<td> GND Masse </td></tr>
<tr>
<td> 5</td>
<td> PD2 </td>
<td> INT0 ext. </td>
<td> TLE Sens 1 </td></tr>
<tr>
<td> 6</td>
<td> PD3 </td>
<td> INT1 ext. </td>
<td> TLE Sens 2 </td></tr>
<tr>
<td> 7</td>
<td> PD4 </td>
<td> digital </td>
<td> HC-SR04 </td></tr>
<tr>
<td> 8</td>
<td> PD5 </td>
<td> digital </td>
<td> HC-SR04 </td></tr>
<tr>
<td> 9</td>
<td> PD6 </td>
<td> pwm </td>
<td> Servo PWM </td></tr>
<tr>
<td> 10</td>
<td> PD7 </td>
<td> digital </td>
<td> Motor 1 Richtung </td></tr>
<tr>
<td> 11</td>
<td> PB0 </td>
<td> digital </td>
<td> TMotor 2 Richtung  </td></tr>
<tr>
<td> 12</td>
<td> PB1 </td>
<td> pwm </td>
<td> M1 PWM </td></tr>
<tr>
<td> 13</td>
<td> PB2 </td>
<td> pwm </td>
<td> M2 PWM </td></tr>
<tr>
<td> 14</td>
<td> PB3 </td>
<td> UART RXD </td>
<td> RFID TTL RDM6300 </td></tr>
<tr>
<td> 15</td>
<td> PB4 </td>
<td> digital </td>
<td> Optoisolator 6N137 für DCC </td></tr>
</table>

<table class="wikitable sortable2">
<tr>
<td> 16</td>
<td> PB5 </td>
<td> digital </td>
<td> reserviert </td></tr>
<tr>
<td> 17</td>
<td> 3V3 </td>
<td> 3,3 Volt Ausgang </td>
<td> reserviert </td></tr>
<tr>
<td> 18</td>
<td> AREF </td>
<td> externe Volt Referenz </td>
<td> reserviert </td></tr>
<tr>
<td> 19</td>
<td> PC0 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 20</td>
<td> PC1</td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 21</td>
<td> PC2 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 22</td>
<td> PC3 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 23</td>
<td> PC4 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 24</td>
<td> PC5 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 25</td>
<td> ADC6 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 26</td>
<td> ADC7 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 27</td>
<td> 5V </td>
<td> 5V </td>
<td> externes 5V Netzteil  </td></tr>
<tr>
<td> 28</td>
<td> PC8 </td>
<td> analog </td>
<td> reserviert </td></tr>
<tr>
<td> 29</td>
<td> GND </td>
<td> GND Masse </td>
<td> reserviert </td></tr>
<tr>
<td> 30</td>
<td> VIN </td>
<td> VIN </td>
<td> externes 6-20V Netzteil  </td></tr>
</table>
