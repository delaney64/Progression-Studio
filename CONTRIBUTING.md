# Contributing to Progression Studio

Thank you for your interest in contributing to Progression Studio! This document provides guidelines and information for contributors.

## Ways to Contribute

### 🐛 Bug Reports
Found a bug? Help us fix it:
1. Check [existing issues](https://github.com/delaneyd/Progression-Studio/issues) first
2. Create a new issue with:
   - Clear title describing the problem
   - Steps to reproduce
   - Expected vs actual behavior
   - Browser and OS version
   - Screenshots if applicable

### 💡 Feature Requests
Have an idea? We'd love to hear it:
1. Check if it's already suggested in issues
2. Open a new issue tagged "enhancement"
3. Describe the feature and its use case
4. Explain why it would benefit users

### 🎵 Musical Enhancements
Music theory improvements are especially welcome:
- New scale types
- Additional chord templates
- Better voice leading algorithms
- Rhythm pattern variations
- Borrowed chord expansions

### 📖 Documentation
Help make the project more accessible:
- Fix typos or unclear explanations
- Add usage examples
- Create tutorials or guides
- Improve code comments

### 🎨 Design Improvements
UI/UX contributions:
- Accessibility enhancements
- Visual design refinements
- Responsive design improvements
- Color scheme alternatives

## Development Process

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Text editor or IDE
- Basic understanding of HTML, CSS, and JavaScript
- (Optional) Git for version control

### Getting Started

1. **Fork the repository**
   ```bash
   # Click "Fork" on GitHub, then clone your fork
   git clone https://github.com/YOUR-USERNAME/Progression-Studio.git
   cd Progression-Studio
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Edit `ProgStudio.html`
   - Test thoroughly in multiple browsers
   - Ensure the file remains self-contained

4. **Test your changes**
   - Open the file directly in browsers
   - Test all affected functionality
   - Verify MIDI export works correctly
   - Check audio preview in different scenarios

5. **Commit your changes**
   ```bash
   git add ProgStudio.html
   git commit -m "Add: brief description of changes"
   ```

6. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

7. **Create a Pull Request**
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Select your branch
   - Provide a clear description of changes

## Code Guidelines

### General Principles
- **Keep it vanilla**: No frameworks, no build tools, no dependencies
- **Single-file architecture**: All code stays in `ProgStudio.html`
- **Progressive enhancement**: Ensure basic functionality works everywhere
- **Performance matters**: Keep the app lightweight and responsive

### JavaScript Style
```javascript
// Use descriptive variable names
const noteFrequency = calculateFrequency(midiNote);

// Comment complex logic
// Convert MIDI note to frequency using A440 reference
function midiNoteToFreq(note) {
  return 440 * Math.pow(2, (note - 69) / 12);
}

// Use const/let instead of var
const immutableValue = 42;
let mutableValue = 0;

// Prefer template literals
const filename = `piano_${key}_${scale}_${bpm}bpm.mid`;
```

### CSS Style
```css
/* Use CSS custom properties for theming */
:root {
  --accent: #6ee7ff;
  --text: #e8eef7;
}

/* Mobile-first responsive design */
.grid {
  display: grid;
  grid-template-columns: 1fr;
}

@media (min-width: 520px) {
  .grid.two { grid-template-columns: 1fr 1fr; }
}
```

### HTML Style
```html
<!-- Semantic HTML5 elements -->
<main>
  <section class="panel">
    <header class="hd">
      <h2>Section Title</h2>
    </header>
  </section>
</main>

<!-- Accessible form controls -->
<label for="key-select">Key</label>
<select id="key-select" aria-label="Musical key selection">
  <option value="C">C</option>
</select>
```

## Testing Checklist

Before submitting a PR, verify:

### Functionality
- [ ] MIDI export produces valid files
- [ ] Audio preview plays correctly
- [ ] All controls update state properly
- [ ] Template application works
- [ ] Randomization respects scale rules
- [ ] Borrowed chords function correctly

### Browser Compatibility
- [ ] Chrome/Edge (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest)
- [ ] Mobile browsers (iOS Safari, Chrome Android)

### UI/UX
- [ ] Responsive design works on mobile
- [ ] All interactive elements have proper hover/focus states
- [ ] Text is readable at all screen sizes
- [ ] Buttons are properly sized for touch
- [ ] Loading states are clear

### Performance
- [ ] File size remains reasonable (< 100KB)
- [ ] No console errors or warnings
- [ ] Smooth animations and transitions
- [ ] Quick response to user interactions

## Musical Accuracy

When adding musical features, ensure:
- **Theory correctness**: Follow established music theory principles
- **Scale accuracy**: Verify interval patterns are correct
- **Chord voicing**: Ensure voicings sound natural
- **MIDI compliance**: Follow MIDI specification standards
- **Notation standards**: Use conventional notation symbols

## Pull Request Guidelines

### Title Format
```
Add: New feature description
Fix: Bug description
Update: Improvement description
Docs: Documentation changes
```

### Description Template
```markdown
## Description
Brief summary of changes

## Changes Made
- Specific change 1
- Specific change 2
- Specific change 3

## Testing
How the changes were tested

## Screenshots (if applicable)
Visual changes before/after

## Related Issues
Fixes #123
```

### Review Process
1. Maintainer reviews code and tests functionality
2. Feedback provided via PR comments
3. You address feedback with additional commits
4. Once approved, changes are merged
5. Your contribution is credited in CHANGELOG.md

## Code of Conduct

### Our Standards
- Be respectful and inclusive
- Accept constructive criticism gracefully
- Focus on what's best for the project
- Show empathy toward others
- Use welcoming and inclusive language

### Unacceptable Behavior
- Harassment or discriminatory language
- Trolling or inflammatory comments
- Personal attacks
- Publishing others' private information
- Unprofessional conduct

## Questions?

Feel free to:
- Open an issue for clarification
- Reach out via GitHub Discussions
- Check existing documentation first

## Recognition

Contributors will be:
- Listed in release notes
- Credited in CHANGELOG.md
- Acknowledged in project documentation

Thank you for helping make Progression Studio better! 🎵
