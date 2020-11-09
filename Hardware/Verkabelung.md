# Hardware 

## Verkabelung des Displays

Display  <->   Raspi Zero W (GPIO--- Pinbezeichnung)

```
VSS -- GND (Pin3)
A  --- GPIO23 (Pin 16)
VDD -- 3V3 (Pin17)
RS --- GPIO24 (Pin 18)
SI --- GPIO10(pin 19)
RSE -- GPIO25(Pin22)
SCL -- GPIO11 (Pin23)
CS --- GPIO08 (Pin24)
K ---- GND (Pin39)
```

## Verkabelung Power Unit. 

Am Raspi gibt es 5V Lötpunkte für die Spannung des StepUP Wandlers
PP1 = +5V
PP6 = GND 

Am Stepup Wandler muss der Jumper P5 geschlossen sein damit der 18650 Geladen wird. Siehe Manual. 












