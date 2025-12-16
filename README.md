# Progression Studio

A browser-based MIDI chord progression builder with real-time audio preview and professional-grade export capabilities. Built with vanilla JavaScript for maximum compatibility and zero dependencies.

![Piano MIDI Progression Builder](https://img.shields.io/badge/MIDI-Export-6ee7ff?style=flat-square) ![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript-a78bfa?style=flat-square) ![Web Audio API](https://img.shields.io/badge/Web%20Audio-API-34d399?style=flat-square)

## Features

### 🎹 Core Functionality
- **Full chromatic key support** - All 12 musical keys with sharp/flat notation
- **Multiple scale types** - Major, natural minor, harmonic minor, melodic minor, dorian, mixolydian, and more
- **Modal borrowing** - Access chords from parallel scales for richer harmonic possibilities
- **Smart chord generation** - Automatic voice leading, inversions, and bass note options

### 🎵 Musical Controls
- **Chord styles** - Triads, 7th chords, 9th chords, suspended chords
- **Voice preferences** - Closed, open, spread voicings
- **Inversion control** - Root position, 1st, 2nd, 3rd inversions, or auto-selection
- **Rhythm patterns** - Whole notes, half notes, quarter notes, eighth notes, arpeggios, and block chords
- **Bass modes** - Root notes, fifth intervals, or octave doubling

### 🎚️ Advanced Features
- **Template library** - Pre-built progressions (I-V-vi-IV, ii-V-I, and more)
- **Randomization** - Intelligent random chord generation within scale
- **Humanization** - Subtle timing and velocity variations for natural feel
- **Velocity modes** - Fixed, accented beats, or fully dynamic
- **Time signatures** - 4/4, 3/4, 6/8, 5/4 support
- **Tempo control** - 40-240 BPM range

### 🔊 Playback & Export
- **Real-time audio preview** - WebAudio API synthesis with configurable octave ranges
- **Loop mode** - Continuous playback for composition workflow
- **MIDI export** - Standard MIDI File format (.mid) with proper track naming
- **Clean file naming** - Exports include key, scale, time signature, and BPM in filename

## Quick Start

### Running Locally

1. Clone the repository:
```bash
git clone https://github.com/delaneyd/Progression-Studio.git
cd Progression-Studio
```

2. Open `index.html` in a modern web browser:
```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

No build process or dependencies required!

### Using a Local Server (Optional)

For development or testing:
```bash
# Python 3
python -m http.server 8000

# Node.js
npx http-server
```

Then navigate to `http://localhost:8000`

## Usage Guide

### Creating Your First Progression

1. **Select your key and scale**
   - Choose from the key dropdown (C, D♭, D, etc.)
   - Pick a scale type (Major, Minor, etc.)

2. **Configure the progression**
   - Set length (1-16 bars)
   - Choose time signature (4/4, 3/4, etc.)
   - Set tempo (BPM)

3. **Build chords**
   - Click individual bars to select chords from the scale
   - Or use "Apply Template" for common progressions
   - Or click "Randomize" for inspiration

4. **Customize the sound**
   - Chord Style: Triads vs extended chords
   - Voicing: Spread of notes across the keyboard
   - Rhythm: How notes are played in time
   - Velocity: Note dynamics

5. **Preview and export**
   - Click "Preview" to hear your progression
   - Toggle loop for continuous playback
   - Click "Export MIDI" to save your work

### Modal Borrowing

Enable "Borrowed Chords" to access chords from parallel scales. For example, in C Major you can borrow chords from C Minor, adding sophisticated harmonic color to your progressions.

### Templates

Built-in templates include:
- **Pop Progression** - I-V-vi-IV (classic pop/rock)
- **Jazz ii-V-I** - Essential jazz cadence
- **50s Progression** - I-vi-IV-V (doo-wop classic)
- **Blues Feel** - I-IV-I-V (12-bar blues foundation)
- **Ascending 4ths** - I-IV-viio-iii-vi-ii-V-I
- **Descending Bass** - I-V/VII-vi-IV (Pachelbel-style)

## Technical Details

### MIDI Implementation
- **Format**: Type 0 MIDI file (single track)
- **Resolution**: 480 PPQ (pulses per quarter note)
- **Track name**: "Piano"
- **MIDI Channel**: 1
- **Note range**: C2-C7 (MIDI notes 36-96)

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

Requires WebAudio API support for playback preview.

### Performance
- File size: ~60KB (single HTML file)
- Memory usage: Minimal (< 5MB runtime)
- No external dependencies or network requests
- Fully offline-capable

## Project Structure

```
Progression-Studio/
├── index.html               # Complete application (HTML, CSS, JS)
├── README.md                # This file
├── LICENSE                  # MIT License
└── CHANGELOG.md             # Version history
```

## Contributing

Contributions are welcome! Here are some ways you can help:

- 🐛 Report bugs via [GitHub Issues](https://github.com/delaneyd/Progression-Studio/issues)
- 💡 Suggest features or improvements
- 🎵 Add new scale types or chord templates
- 📖 Improve documentation
- 🎨 Enhance UI/UX design

### Development Guidelines

1. Keep it vanilla - No frameworks or build tools
2. Maintain single-file architecture
3. Test across browsers before submitting PRs
4. Follow existing code style and conventions
5. Document new features thoroughly

## Roadmap

Potential future enhancements:
- [ ] Additional rhythm patterns (syncopation, swing)
- [ ] Drum/percussion track layer
- [ ] Save/load progression presets to localStorage
- [ ] Dark/light theme toggle
- [ ] Export to other formats (MusicXML, ABC notation)
- [ ] Chord chart visualization
- [ ] MIDI input for real-time recording

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Built with passion for music theory and web technology. Inspired by:
- Music theory fundamentals from Berklee College of Music
- MIDI specification standards from MIDI Association
- WebAudio API capabilities

## Contact

**Project Link**: [https://github.com/delaneyd/Progression-Studio](https://github.com/delaneyd/Progression-Studio)

---

Made with 🎵 for musicians and developers
