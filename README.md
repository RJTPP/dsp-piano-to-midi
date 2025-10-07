# 🎵 Piano → MIDI (Monophonic Transcription)

A **deterministic DSP pipeline** to convert monophonic piano sound into MIDI notes.

Core stages:

* **Framing + YIN f₀ estimation**
* **Stabilization** (median filter + doubling/halving guard)
* **Onset detection** via spectral flux
* **Hysteresis rounding + min-duration merge**
* **Hz → MIDI mapping**, with **key snapping**
* **MIDI rendering**
