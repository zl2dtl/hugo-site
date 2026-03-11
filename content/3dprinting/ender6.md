---
title: "Ender 6 Build Log"
layout: page
---

This is the first entry in what will probably be a long running build log for the Ender 6 we're getting up and running at Zero Waste. The goal is simple enough in theory: get a printer running reliably enough that it can live at the shop and be used at repair cafes to print whatever parts are needed to keep things out of landfill. In practice, as with most things, it's been a bit more involved than that.

The printer came in supposedly not working, which is about as specific as the brief gets. Someone had already begun work on it before I got involved, following [this Klipper guide for the Ender 6](https://github.com/zimmertr/Ender-6-Klipper-Guide) as the basis for the build. So the plan was already set: Ender 6 with Klipper. I came in partway through and we've been working on it together since.

First issue out of the gate was the display macros, none of them were working. Had to dig into the config, modify what was there, and write new macros from scratch for the basics like purging and loading filament. Not the most glamorous work but it needed doing before anything else was going to make sense.

The printer did manage to produce a Benchy at some point, which counts as progress. Someone (me) got impatient and bumped the speed up to 800%, which is one way to find out where your tuning falls short. It needs work.

The bigger problem has been the BL Touch. The Ender 6 has a daughter board that handles connections for things like the probe, which sounds convenient until you realise it only passes through three of the five BL Touch pins. Signal lines, no power. The BL Touch needs 5v to function reliably and the daughter board only puts out 3.3v, so the probe was never going to work 100% properly regardless, though Creality supposedly thought it would have. On top of that, the original BL Touch had to come off entirely because the retraction mechanism had failed and it wasn't retracting at all, which turned out to be a power issue for exactly that reason. Also, the probe on the printer originally had no cable with it, so we could not connect anything to the BL Touch at all. 

I brought in my own BL Touch along with a cable, which solved the probe problem but left the motherboard end without a connector. I carefully removed the original wires hoping the plastic connector housing would survive intact, which it did, mostly. To reconnect everything properly I've ordered some pre-crimped JST cables to re-seat into the old connector body, along with a 5-pin JST cable as a backup in case the connector housing doesn't cooperate.

The plan once the cables are sorted is to run some Cat5e ethernet cable or similar between the BL Touch's connector at the extruder head and the motherboard, bypassing the daughter board entirely and giving the probe a clean 5v feed directly. That should be the end of the BL Touch saga, fingers crossed.

The cables have arrived. I'm back at Zero Waste on Saturday. More then.