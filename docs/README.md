# ep_booster

KiCad project for EP Booster

---

The idea with this project is to have it in one place, with some "standards" like to view everything in KiCad and export
for manufacturing.

As a bassist, I'm using EP Booster as always on pedal in vintage mode without a boost, and it gives a nice warmth to my
custom bass with jazz pickups, and better thump with my Squier VM Precision with Wilde P-46 pickup.

~~What I want to do as a first version is to have the whole thing working the same as my EP Booster 70th Thomann
Aniversiry, and then strip away the parts that are for boost and just leave the vintage part in there so I can put it
into my basses, thus removing one pedal from signal chain.~~

Since I already have the pedal, first version will actually be ready to put into the bass, so it will use a trim pot

I guess the eq part will last a long time in bass, since I was running it as a pedal for 3-4 months as always on
on battery, and with stripped components (especially LED), it should last even longer. I'll have to do measurements
and write that here.

---

Resources for the project:

- https://aionfx.com/news/tracing-journal-xotic-ep-booster-v2/
- https://www.taydakits.com/instructions/ep-booster/pages/designators-and-components--20
- https://revolutiondeux.blogspot.com/2012/01/xotic-ep-booster.html
- http://toshi.life.coocan.jp/review/en_diy_booster_surface_mount.html
- https://www.amp-fx.de/ep-preamp-booster-en.htm (this one is interesting because it has more caps to change the
  characteristic of the vintage mode)
- https://guitar-electronics.eu/en_US/p/EP-BOOSTER-kit-ULTRA/408

---

I've copied the AionFx to KiCad but without R15 and LED1 since I'm not planning to put that into the bass, but that
can be added later, and we can just bypass it, or rather not use it.

Since I'll be using trimmer instead of potentiometer, it doesn't matter if it's audio/linear/log/reverse audio, I'm
planning to keep it at lowest value anyway, so it works without a boost. But if a signal from bass is weak, it can serve
as a boost to get hotter signal out of the bass. This will consume more battery.

---

I'll try to keep the footprint of the PCB less than the 9V battery size, the idea being that you can have 9V battery
slots in the bass, where 1 is the battery itself and other is this in the shape of another battery. I'll probably have
to create a 3D holder for it, but that should be easy once everything is working.

---

TODO:

1. Add bypass switch that also disconnects the battery, so it's easy to bypass on low battery. This can even be soldered
   to push/pull pot
2. Add low battery indicator (but that can be separate circuit). This needs to be tested at how low voltage does the
   audio signal degrade the circuit.
3. Add LED and current limiting resistor R15 to the schematic so it's complete, but it doesn't have to be on the board
4. Add mounting holes for screws M3, one or two should be enough to keep it in place
5. Make 3D case that should be the same size as battery, so positioning can be like two batteries one next to other, but
   should keep in mind the switches and pot, they should be available for easy modification.