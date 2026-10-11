# SF2 Mixer

Multi-timbral SoundFont (SF2) player for **Android**, built for **live performance**.

Load your own `.sf2` instruments, play them from a USB or Bluetooth MIDI keyboard, mix up to **8 independent channels**, and route everything through a master bus with reverb and cutoff.

---

## Features

- **Up to 8 channels**, each with its own SF2 timbre  
- **Volume faders** with dB scale and real audio level meters  
- **Mute (M)** and **Solo (S)** per channel  
- **Attack** and **Release** knobs per channel  
- **Master**: volume, reverb, cutoff  
- **PAD** mode: sustained pad loop locked to the first note played  
- **MIDI Learn**: map keys/CCs to mute, solo, faders, and knobs  
- **Presets**: save and reload the full mixer setup  
- **SF2 library**: import once, assign to channels from a list  
- **USB audio interface** support (e.g. Focusrite Scarlett) with selectable buffer / latency  
- Landscape UI optimized for stage use  
- Built with **Jetpack Compose**, **FluidSynth** (NDK), and **AAudio** for low-latency playback  

---

## Requirements

- Android **8.0+** (API 26)  
- **arm64-v8a** device (most modern phones)  
- Optional: USB/Bluetooth MIDI keyboard  
- Optional: USB audio interface  

---

## How to use

1. Open the app (landscape).  
2. Use **Files** in the top bar to import `.sf2` files into the library.  
3. Press **+** to add a channel and pick a timbre from the library.  
4. Connect a MIDI keyboard — the app tries to auto-connect.  
5. Adjust volume, attack, release; use **M** / **S** for mute and solo.  
6. Save a **preset** to restore the full setup later.  

**Close a channel:** long-press the channel strip → confirm.

---

## Build

1. Open the project in **Android Studio**.  
2. Sync Gradle.  
3. Install **NDK** + **CMake** if prompted.  
4. Run on a physical **arm64** device (or build a signed release APK / AAB).  

```bash
./gradlew assembleRelease
