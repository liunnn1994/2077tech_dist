# Supplemental interface audio

Sources: Kenney, **Interface Sounds (1.0)** and **Sci-Fi Sounds (1.0)**,
CC0 (commercial use allowed).

- Author: https://kenney.nl/assets/interface-sounds
- Download mirror: https://opengameart.org/content/interface-sounds
- Archive: https://opengameart.org/sites/default/files/kenney_interfaceSounds.zip
- Original license: [LICENSE.txt](LICENSE.txt)
- Sci-Fi source: https://kenney.nl/assets/sci-fi-sounds
- Sci-Fi archive: https://opengameart.org/sites/default/files/sci-fi_sounds.zip
- Sci-Fi license: [LICENSE-scifi.txt](LICENSE-scifi.txt)

| Local file | Original | Use |
| --- | --- | --- |
| transition-home.ogg | Sci-Fi: doorClose_002.ogg | Mechanical closure on return to the first section |
| transition-portfolio.ogg | Sci-Fi: computerNoise_000.ogg | Electronic data pulse on entering portfolio |
| transition-particles.ogg | Sci-Fi: forceField_000.ogg | Energy-field sweep before rings/contact section |
| terrain-scan.ogg | select_002.ogg | Accepted terrain click / scan |
| particle-morph.ogg | Sci-Fi: doorClose_000.ogg | Short mechanical latch when the last section's logo changes |
| ui-confirm.ogg | confirmation_001.ogg | External project link / language change |

Edits: mono 44.1 kHz Vorbis, -22 LUFS normalization, 15 ms attack.
Scan/confirmation retain 120 Hz high-pass / 5 kHz low-pass, -6 dBTP ceiling
and 100 ms release; scan uses 0.8x tempo, confirmation uses original tempo.

The four Sci-Fi clips use 160 Hz high-pass / 4.2 kHz low-pass and -8 dBTP
ceiling, with pitch and speed reduced together. Morph: 0.9x, 500 ms,
120 ms release. Home: 0.85x, 630 ms, 180 ms release. Portfolio: original
starts at 350 ms, 0.9x, 480 ms, 180 ms release. Particles: 0.85x, 850 ms,
180 ms release. These replace the previous melodic/bouncy interface samples.
All clips are one-shots and share the existing master mute/visibility controls.

Global music-highq.ogg and room.ogg are no longer registered or downloaded.
Other original audio remains in use. Scene loop volume changes use a 150 ms
time constant (roughly 450 ms to settle), preserving tails across visual seams.
New section cues use 35%/65% hysteresis and a 1.2 s per-clip cooldown.
