# MIDI Goblin

MIDI Goblin is an open-source hardware MIDI controller designed and developed by Andrew Crawford to enhance MIDI capabilities for musicians and producers. It provides patch management, arpeggiation, sequencing, and other MIDI features for synthesizers and controllers that lack advanced MIDI functionality. It was launched on Kickstarter to address the limitations of synthesizers and MIDI controllers that lack features like patch storage, arpeggiation, and advanced sequencing. 

## Features
- **Patch Saver**: Save and load patches for MIDI synthesizers and controllers.
- **Arpeggiator**: Real-time arpeggiation with configurable speed and modes.
- **Sequencer**: 32-step MIDI sequencer for creating and playing patterns.
- **MIDI LFO**: Modulate any MIDI CC number with customizable waveforms.
- **Auto-Chord and Arp-Note**: Generate chords and arpeggios for dynamic performances.
- **CC Remapping**: Remap outgoing MIDI CC messages to simplify synth programming.

## Getting Started

### Requirements
- **Hardware**: ESP32 Doit Devkit V1
- **Software**:
  - [PlatformIO](https://platformio.org/) (Recommended)
  - [Arduino IDE](https://www.arduino.cc/en/software) (Optional)
- **Libraries**:
  - Adafruit GFX Library
  - Adafruit SH110X Library
  - MIDI Library
  - SPI
  - Wire
  - SD

### Installation Instructions
Before building the project, ensure you have **PlatformIO** installed. PlatformIO simplifies dependency management and builds for embedded systems.

#### Install PlatformIO via pip
If you don't already have PlatformIO installed, run:
```bash
pip install platformio
```
This will install PlatformIO globally. You can then verify the installation with:
```bash
pio --version
```

#### Build and Upload
1. Clone this repository:
   ```bash
   git clone https://github.com/Greendogo/MIDI_Goblin.git
   cd MIDI_Goblin
   ```
2. Install dependencies:
   ```bash
   pio pkg install
   ```
3. Build the project:
   ```bash
   pio run
   ```
4. Upload the firmware to the ESP32:
   ```bash
   pio run --target upload
   ```
###Directory Structure
   ```bash
   MIDI_Goblin/
  ├── src/                      # Source code
  │   ├── build/                # PlatformIO build artifacts
  │   ├── data/                 # Data files
  │   ├── *.cpp                 # C++ source files
  │   ├── *.h                   # Header files
  │   └── midi_goblin.ino       # Main firmware file
  ├── .gitignore                # Git ignore file
  ├── platformio.ini            # PlatformIO configuration
  └── README.md                 # Project documentation
  ```