# EP Booster

![v1.0.0 image](img1_v1_0_0.jpg)

![v1.0.0 image](img2_v1_0_0.jpg)

---

The idea with this project is to have everything on one place, with some "standards" like to view everything in KiCad
and export for manufacturing.

As a bassist, I'm using EP Booster as always on pedal in vintage mode without a boost, and it gives a nice warmth to my
custom bass with jazz pickups, and better thump with my Squier VM Precision with Wilde P-46 pickup.

Since I already have the pedal, first version will actually be ready to put into the bass, so it will use a trim pot,
but that can be wired onto a 10k pot if you want to have an "interface" to boost.

I guess the battery for eq part will last a long time in bass, since I was running it as a pedal for 3-4 months as
always-on on battery, and with stripped components (especially LED), it should last even longer. I'll have to do
measurements and write that here.

---

## Usage

If you want Vintage mode (like me) without a boost, use 10K resistor instead of the trim pot, and you can leave out male
pin headers, this will make sure +3dB is off and vintage mode is on.

I've made just the first board with that, so I can test it, but my plan was to use it without boost and with vintage
mode on so next ones I solder will be without those two components, and I'll just put 10K resistor there.

Use two jumper connectors to connect pin headers for bright/boost.

---

## Decisions

Why this board uses pin header connectors:

1. It's cheaper than a switch
2. Smaller footprint (in mm²), which is important in a board this compact
3. The pedal will be used probably how you set it up once, so you won't change that

The only benefit of a switch is that it's more practical, and you won't lose jumper shunt. But since I soldered it only
on the first board, and I'm not planing to use that anyway, I won't solder it anymore.

---

Resources for the project:

- https://aionfx.com/news/tracing-journal-xotic-ep-booster-v2/ (the pedal I've made is 100% based on this)
- https://www.taydakits.com/instructions/ep-booster/pages/designators-and-components--20
- https://revolutiondeux.blogspot.com/2012/01/xotic-ep-booster.html
- http://toshi.life.coocan.jp/review/en_diy_booster_surface_mount.html
- https://www.amp-fx.de/ep-preamp-booster-en.htm (this one is interesting because it has more caps to change the
  characteristic of the vintage mode)
- https://guitar-electronics.eu/en_US/p/EP-BOOSTER-kit-ULTRA/408

---

I've copied the AionFx to KiCad but without R15 and LED1 since I'm not planning to put that into the bass, but that
can be added later, and we can just bypass it or leave the components out, or rather not use it. I hope that won't
affect tone because it might lower the voltage a bit. I'll test with my pedal to see if there's any difference and make
changes to the schematic if necessary, but I don't need LED so if it does lower voltage and affects tone, I'll have to
find a workaround.

Since I'll be using trimmer instead of potentiometer, it doesn't matter if it's audio/linear/log/reverse audio, I'm
planning to keep the gain at the lowest value anyway (so highest value cap - 10kOhm), so it works without a boost. But
if a signal from bass is weak, it can serve as a boost to get hotter signal out of the bass. This will consume more
battery.

---

[Here's more info about EP Booster Vintage mode.](ep_booster_info.md)

---

TODO:

1. ✅ Make 3D case that should be the same size as battery, so positioning can be like two batteries one next to other,
   but should keep in mind the switches and pot, they should be available for easy modification.
2. ✅ Add bypass switch, so it's easy to bypass on low battery. This can even be soldered to push/pull pot
3. Add LED and current limiting resistor R15 to the schematic so it's complete, but it doesn't have to be on the board
4. Experiment with different capacitor values like the one from amp-fx, to see if there's anything better or is it maybe
   per bass better
5. ✅ Voltage doubler combined with EP booster for more headroom. Maybe put a switch there so you can choose if you want
   to use 9 or 18v.
   Schematic is made and I have it working, it produces 17.5v. I'll create a separate scheme for it, I don't think
   there's a need to use 18v onboard. The sound is there and there's probably plenty of gain. I didn't measure that yet.
6. test how much boost I get from every 1K resistence, or if there's like 16db boost, measure when I get every
   -1 db so I can say for example I want exactly 10db boost. Also test with 18V battery since it has bigger headroom.
   Test when I have +3db boost on as well, is it really 3db or what. Test db output in bypass and switched on without
   any boost to see if there is in fact any boost because my ears say there is.
7. See if it's possible to make it work on a 3 way switch, with positions off, on without boost (10k resistor), on with
   boost (some resistance, maybe that should stay on trim pot)
8. Replace C2 from 47uF to 10uF. I've opened my EP Booster and checked for value of C7 (my C2) and saw that it wasn't
   47uF but 12uF (10uF +- 20% tolerance). Why I noticed this is because images from aixon tracing show six of the same
   caps and one different. The six are red ones from Jackcon (35V -40 to 105 degrees C, 5mm wide, 7.2mm high, 2.5mm
   lead spacing). So I guess that's the only part to change and test if it works the same as original.

---

From tadyakits - worth experimenting for sound change

The original bass and treble switches do not have noticeable effect. To remove more bass, reduce C3 capacitance (e.g.
0.1 uF). To remove more treble, increase R7 resistance (e.g. 33k).