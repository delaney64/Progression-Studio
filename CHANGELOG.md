# Changelog

All notable changes to Progression Studio will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-12-14

### Added
- Initial release of Progression Studio
- Complete MIDI chord progression builder
- Real-time audio preview with WebAudio API
- Support for 12 chromatic keys with sharp/flat notation
- Multiple scale types (Major, Minor, Dorian, Mixolydian, etc.)
- Modal borrowing for parallel scale chord access
- Chord style options (Triads, 7th, 9th, Sus chords)
- Voice preference controls (Closed, Open, Spread)
- Inversion options (Root, 1st, 2nd, 3rd, Auto)
- Rhythm patterns (Whole, Half, Quarter, Eighth, Arpeggios, Block)
- Bass mode controls (Root, Fifth, Octave)
- Humanization for natural timing variation
- Velocity modes (Fixed, Accented, Dynamic)
- Time signature support (4/4, 3/4, 6/8, 5/4)
- Tempo control (40-240 BPM)
- Built-in chord progression templates
- Randomization with scale-aware chord selection
- Loop mode for continuous preview
- Professional MIDI export with proper formatting
- Clean filename generation with musical metadata
- Fully responsive UI with modern design
- Single-file architecture (no dependencies)
- Offline-capable web application

### Technical Details
- MIDI Format: Type 0 (single track)
- MIDI Resolution: 480 PPQ
- Note range: C2-C7 (MIDI 36-96)
- File size: ~60KB
- Zero external dependencies

---

## Future Versions

### [Unreleased]
Ideas and potential features for future releases:

#### Planned
- Save/load progression presets
- Additional rhythm patterns (swing, syncopation)
- Chord chart visualization
- Theme toggle (dark/light mode)

#### Considering
- Drum/percussion track layer
- MIDI input for recording
- Export to MusicXML format
- Extended chord voicings library
- Custom scale creation
- Progression analysis tools

---

[1.0.0]: https://github.com/delaneyd/Progression-Studio/releases/tag/v1.0.0
