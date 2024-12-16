# ep_booster

KiCad project for EP Booster

---

The idea with this project is to have it in one place, with some "standards" like to view everything
in KiCad and export for manufacturing.

As a bassist, I'm using EP Booster as always on pedal in vintage mode without a boost, and it gives
a nice warmth to my custom bass with jazz pickups, and better thump with my Squier VM Precision with
Wilde P-46 pickup.

What I want to do as a first version is to have the whole thing as a pedal, and then strip away the
parts that are for boost and just leave the vintage part in there so I can put it into my basses,
thus removing one pedal from signal chain.

---

Resources for the project:

- https://www.taydakits.com/instructions/ep-booster/pages/designators-and-components--20
- https://revolutiondeux.blogspot.com/2012/01/xotic-ep-booster.html
- http://toshi.life.coocan.jp/review/en_diy_booster_surface_mount.html
- https://www.amp-fx.de/ep-preamp-booster-en.htm (this one is interesting because it has more caps to change the
  characteristic of the vintage mode)

---

From the first source, here's the BOM

Capacitors

- C1 47n 47NF 100V 5% POLYESTER FILM BOX TYPE CAPACITOR
- C2 10u 10UF 50V ELECTROLYTIC CAPACITOR 5X11MM
- C3 10u 10UF 50V ELECTROLYTIC CAPACITOR 5X11MM (Original)
- C3 0.1u 0.1UF 50V ELECTROLYTIC CAPACITOR 5X11MM  (Remove more bass)
- C4 100u 100UF 35V ELECTROLYTIC CAPACITOR 6X11MM
- C5 3.3n 3.3NF 100V 5% POLYESTER FILM BOX TYPE CAPACITOR
- C6 10u 10UF 50V ELECTROLYTIC CAPACITOR 5X11MM
- C7 10u 10UF 50V ELECTROLYTIC CAPACITOR 5X11MM
- C8 47u 47UF 25V ELECTROLYTIC CAPACITOR 5X11MM

Diode

- D1 1N4148 1N4148 SWITCHING SIGNAL DIODE

Transistors

- Q1 J201 SMD SOT-23 J201 JFET N-CHANNEL TRANSISTOR
- Q2 2N5088 2N5088 GERENAL PURPOSE TRANSISTOR

Resistors

- R1 1M 1M OHM 1/4W 1% METAL FILM RESISTOR
- R2 33k 33K OHM 1/4W 1% METAL FILM RESISTOR
- R3 1M 1M OHM 1/4W 1% METAL FILM RESISTOR
- R4 50k Trimmer 50K TRIMMER POTENTIOMETER
- R5 4.7k 4.7K OHM 1/4W 1% METAL FILM RESISTOR
- R6 1k 1K OHM 1/4W 1% METAL FILM RESISTOR
- R7 15k 15K OHM 1/4W 1% METAL FILM RESISTOR  (Original)
- R7 33k 33K OHM 1/4W 1% METAL FILM RESISTOR  (Remove more treble)
- R8 10k 10K OHM 1/4W 1% METAL FILM RESISTOR
- R9 1M 1M OHM 1/4W 1% METAL FILM RESISTOR
- R10 10k 10K OHM 1/4W 1% METAL FILM RESISTOR
- R11 10k 10K OHM 1/4W 1% METAL FILM RESISTOR
- R12 47k 47K OHM 1/4W 1% METAL FILM RESISTOR
- R13 100 100 OHM 1/4W 1% METAL FILM RESISTOR

Potentiometer

- GAIN 10k-C 10K OHM ANTI-LOG POTENTIOMETER

Switches (top mounted)

- S1 (Bass)       MINI TOGGLE SWITCH SPDT ON-ON
- S2 (Treble)     MINI TOGGLE SWITCH SPDT ON-ON

Switches (inside mounted)

- S1 (Bass)       MINI SLIDE SWITCH SPDT ON-ON
- S2 (Treble)     MINI SLIDE SWITCH SPDT ON-ON