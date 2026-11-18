# N3VE by VRCVS

**A generative ambient panel for [Plinky 12](https://plinky12.com)** (designed for the Chords faceplate), ported from N3VE, the norns script by VRCVS.

Snow falls in the sky and plays low notes when it lands. The tears answer with a melody. A third voice is yours, on a keyboard that always fits the chord: play a phrase and the tears reply. Chords change at the end of the bar, so you always stay in time.

## Features

- **3 voices**, each with its own sound, octave, mute and MIDI channel: **snow** (white), **tears** (cyan), **live** (pink)
- **Chords on the top row**: tap a degree and the chord changes at the end of the bar; or let the progression run (1, 2, 4 or 8 bars per chord), with freeze
- **Three styles** for the tears: cell (a short motif that varies), arpeggio (with direction), snow
- **Tap the sky** to drop your own flakes; hold to repeat them on the grid
- **Live keyboard** on rows 9–14 with pressure and glide, always in the current chord
- **Call and response**, on by default: the tears learn your phrase and answer it (can be switched off)
- **12 scales** and any key, each with its own colour; density, wind, grid and 6 sound/motion parameters
- **Any sound on every voice**: factory and saved presets, plus your own presets and multisample banks from the SD card
- **MIDI out** per voice (Plinky only, Plinky + MIDI, MIDI only), with aftertouch from the live keyboard
- **Song save/load**: settings, the three sounds and the mix

## Install

1. Open the [Plinky 12 Code Editor](https://plinky12.com/ide.html) in Chrome.
2. Start a blank panel and paste the contents of [`src/n3ve.cpp`](src/n3ve.cpp).
3. Select **Chords** as the faceplate, press **Test** to try it in the emulator (hold ▶ for a moment to start).
4. Connect your Plinky 12 via USB and press **Flash**. Panels open in other IDE tabs are flashed together.
5. Power on holding the bottom-row pad shown for N3VE in the IDE diagram.

## Manual

- English: [`docs/N3VE_manual_EN.pdf`](docs/N3VE_manual_EN.pdf)
- Italiano: [`docs/N3VE_manuale_IT.pdf`](docs/N3VE_manuale_IT.pdf)

## Notes

- The Plinky keeps the samples of all loaded sounds in 14 MB of flash. To use **3 of your own banks at once**, build them in the [Bank Builder](https://vrcvs.github.io/plinky12_bank_builder/) with **Banks loaded together: 3** (about 4 MB each). The same bank on several voices counts once; factory sounds are small.
- Beta: tested in the Plinky 12 emulator. Use at your own risk: custom firmware can always be restored from the Plinky 12 firmware page.

## Credits

- Port of **[NEVE](https://github.com/vrcvs/NEVE)**, the norns script by VRCVS (MIT).
- **Plinky 12** by mmalex and Making Sound Machines.
- N3VE by **VRCVS** (Filippo Rieder) – Instagram [@vrcvs](https://www.instagram.com/vrcvs). Written with the help of Claude (Anthropic).

## License

[MIT](LICENSE)

---

### In italiano

N3VE è un pannello custom generativo per Plinky 12, porting dello script norns NEVE: la neve cade e suona note basse quando tocca terra, le lacrime rispondono con una melodia, e la terza voce la suoni tu su una tastiera sempre nell'accordo. Installazione: incolla `src/n3ve.cpp` nel Code Editor di plinky12.com, prova con **Test**, poi **Flash**. Manuale completo in [`docs/N3VE_manuale_IT.pdf`](docs/N3VE_manuale_IT.pdf).
