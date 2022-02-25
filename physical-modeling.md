# Physical Modeling

### Resources
 - [Paper on strings](https://tel.archives-ouvertes.fr/tel-00349920/document)
 - [Interesting KVR discussion](https://www.kvraudio.com/forum/viewtopic.php?t=488332&sid=362d4e415904ffb46072c29dc66681a7)
 - Madrona Labs [kaivo overview](https://madronalabs.com/products/kaivo). Another [here](https://youtu.be/8elZ_HaMO00)
 - Look at all Madrona Labs instruments
 - [Great Reaktor Model](https://youtu.be/kLkPvmr93K8)

---

## NESS Project
 - [Website](http://www.ness.music.ed.ac.uk/)
 - [Overview video](https://youtu.be/W9nMbtIjygM)
 - [Good Youtube Channel](https://www.youtube.com/user/AAGedinburgh/videos)

## Audio Modeling

### Notes
 - [Entire thesis](https://hal.archives-ouvertes.fr/tel-01219693/document)
 - [Discussion of technology](https://audiomodeling.com/about-us/technology/)
 - [Background on Audio Modeling people](https://audiomodeling.com/about-us/people/)
 - [Interview both founders](https://youtu.be/i-WStJKN4TA)
 - Modeling is done with [digital waveguide synthesis](https://ccrma.stanford.edu/~jos/swgt/)
 - Added parameters for real-time control of bow speed, bow pressure, bow position, vibrato, portamento, harmonics, tremolo, etc
 - More information [here](https://audiomodeling.com/about-us/technology/swam-s/)

## Bowed String Physics Summary

The bow allows the player to input energy continuously and so to maintain a note. This affects the timbre too: after a pluck, the high harmonics fade away quickly, leaving only the fundamental and some weak lower harmonics, while bowing maintains the rich harmonic spectrum.

The action of the bow as it drives the strings is a regular cycle of stick-slip-stick-slip. This involves some interesting properties of friction (the force that makes things difficult to slide).

The bow-string interaction is important for another reason. Through a limited range of pressure applied by the player, the cycle of stick and slip is governed by the standing wave in the string. When this cycle happens, the motion of the string is almost exactly periodic, and therefore the string makes a sound with an almost exact harmonic spectrum. This means that any inharmonic effects of the string are reduced by bowing, which is not the case when the string is plucked.

Helmholtz motion is the name given to the idealized motion of the string during stick and slip cycles.

SWAM-S models this complex system by using the Digital Waveguide Synthesis conceived by Prof. Julius O. Smith, exploiting a complex friction model, and adding several elements taken from the SWAM technology created for the Woodwinds instruments. In combination, these elements improve the realism of the timbre and the overall behaviour of the instrument.

### KVR quote from founder

The technology used in our instruments is indeed a combination of different techniques.
I started in 2007 with a technology called SWT - Synchronous Waves Triggering (a MultiVector Samples ReSynthesis) which was my first attempt to model samples in realtime. These instruments (SaxBrothers) were developed on Native Instrument Kontakt platform. Kontakt (that is a very good platform and basically an advanced sampler perfect for sample libraries) is non the best tool for this Synthesis technique, so I decided to make a proprietary engine. In 2009 I met Emanuele Parravicini and together begun the development of the SWAM engine.
SWAM, Synchronous Waves Acoustic Modeling (or now we prefer Synchronous Waves Audio Modeling) adds concepts of Physical Modeling to the MultiVector Sample technique. We made different versions of the engine, each one more suitable for a specific family of instruments.
Each version has different balance between Sample and Physical Modeling.
Reeds, that use engine version 1, is basically a Multivector Sample engine with some Physical Modeled Resonance elements and Behavioral modeling techniques.
Flutes use version 2 with a bigger component of physical modeling tecnique than sampling and in our opinion represent the best example of mixing between both techniques because we have sampled the lower dynamics on the first octave only and all other notes and dynamics are obtained by modeling this limited sampled material, through the obtainment of Overtones.
Lastly, Bowed Strings (our recent product) are made mainly with Physical Modeling approach. We decided to 100% model Bowed Strings by WaveGuide Synthesis (a Physical Modeling method conceived by Prof. Julius O.Smith) because it was very difficult obtain the BowPressure parameter (Very important expression control) with others SWAM techniques.

---

## Physical Audio

### Notes
 - [SMC 2021 Keynote](https://youtu.be/JcMR1FVcpF8)
 - [Timbre 2020 Keynote](https://youtu.be/6Bx0DNiNvFk)
 - [Code samples](https://physicalaudio.co.uk/testing-simd-performance-on-apples-new-m1-processor/)
 - Detrailer technical details [here](https://physicalaudio.co.uk/derailer-tutorial-driver/) and [here](https://physicalaudio.co.uk/derailer-tutorial-resonator/)
 - Preparation details [here]
