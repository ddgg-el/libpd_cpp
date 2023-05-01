# Libpd RtAudio Example.

This repository shows how to use libpd embedded in a cpp program using the RT audio.

The pd Patch is a simple ring modulator which receives the modulation frequency from cpp. The patch also comunicates with the cpp program  via a `send` object with the label `cursor`.