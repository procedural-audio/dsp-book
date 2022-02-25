# Physical Modeling

### Resources
 - [Paper on strings](https://tel.archives-ouvertes.fr/tel-00349920/document)
 - [Interesting KVR discussion](https://www.kvraudio.com/forum/viewtopic.php?t=488332&sid=362d4e415904ffb46072c29dc66681a7)
 - [Kaivo overview](https://madronalabs.com/products/kaivo). Another [here](https://youtu.be/8elZ_HaMO00)

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

---

## Physical Audio

### Notes
 - [SMC 2021 Keynote](https://youtu.be/JcMR1FVcpF8)
 - [Timbre 2020 Keynote](https://youtu.be/6Bx0DNiNvFk)
