<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/a9e88348-1b32-4ecd-a284-3160b4e9995a

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

# 🎵 AI Song Maker & Vocal Studio (Raag Studio)

**An AI-powered music production workstation, vocal studio, and songwriting companion built with React, TypeScript, the Web Audio API, and Google Gemini 2.5 Flash.**

Raag Studio is a browser-based digital audio workstation (DAW) designed to bring songwriting, music composition, vocal processing, and audio production together in one creative environment.

It combines Indian classical and Western music theory, procedural audio synthesis, an interactive MIDI piano roll, intelligent lyric analysis, and AI-assisted songwriting tools.

Whether you're creating Bollywood romantic ballads, Punjabi pop, Sufi-inspired compositions, lo-fi beats, or cinematic soundtracks, Raag Studio provides tools to help you develop your musical ideas from initial inspiration to a finished audio project.

## ✨ Key Features

### 🎛️ 1. Multitrack Audio Engine & Piano Roll

Create and arrange music using a browser-based synthesizer powered by the Web Audio API.

- Client-side procedural audio synthesis.
- Interactive MIDI piano roll with a visual note grid.
- Add, delete, resize, and arrange musical notes.
- Octave switching and zoom controls.
- Real-time playback cursor synchronization.
- Support for MIDI Type 0 and Type 1 exports.
- Multitrack sequencing and individual instrument controls.

**Supported instruments:**

- **Sitar:** Resonant plucked-string synthesis with sympathetic resonance.
- **Bansuri:** Breath-inspired flute synthesis with subtle pitch vibrato.
- **Harmonium:** Warm, layered reed-style synthesis.
- **Tanpura:** Continuous drone with harmonic overtones.
- **Dholak and Tabla:** Procedurally synthesized Indian percussion.
- **808 Sub-Bass:** Deep bass tones with soft-clipping saturation.

### ✍️ 2. AI Lyrics Studio

Write, analyze, and improve song lyrics with intelligent songwriting assistance.

- Generate lyrics from topics, emotions, and creative prompts.
- Detect phonetic rhymes and categorize rhyme relationships.
- Identify rhyme schemes such as AABB, ABAB, and AAAA.
- Analyze syllables and rhythmic stress.
- Support Radif and Qafia analysis for Urdu and Hindi poetic forms.
- Generate context-aware lyric suggestions using Google Gemini.
- Explore song structures, including verses, choruses, and bridges.
- Insert suggested lyric lines directly into the editor.

### 🎼 3. Music Theory & Raga Studio

Explore Western music theory and Indian classical musical traditions.

- Generate and audition chord progressions.
- Experiment with major, minor, modal, and pentatonic scales.
- Explore Indian classical raga-inspired scale structures.
- Visualize melodic contours and pitch transitions.
- Analyze intervals and melodic movement.
- Develop musical ideas using different harmonic and melodic approaches.

**Supported Western scales and modes include:**

Major, Natural Minor, Harmonic Minor, Melodic Minor, Dorian, Phrygian, Lydian, Mixolydian, Locrian, Blues Minor, Major Pentatonic, and Minor Pentatonic.

**Supported Indian raga-inspired scales include:**

Bilawal, Kalyan, Khamaj, Kafi, Asavari, Bhairav, Bhairavi, Todi, Marwa, and Poorvi.

### 🎚️ 4. Multitrack Mixer & Mastering Suite

Mix and refine your music using dedicated channel controls and audio effects.

- Individual channel volume faders.
- Decibel gain metering.
- Stereo panning.
- Solo and mute controls.
- Three-band equalization.
- Compressor with adjustable threshold, ratio, attack, and release.
- Algorithmic reverb and tape delay.
- Master limiting and soft-clipping maximization.
- Real-time waveform and audio spectrum visualization.

### 🎤 5. Vocal Studio & Audio Cleaner

Process vocal recordings and experiment with audio effects.

- Pitch correction and vocal tuning.
- Formant and pitch-shifting effects.
- Vocal warmth and saturation.
- Doubler and chorus effects.
- Background noise reduction.
- Room hum suppression.
- Transient shaping.
- Live microphone monitoring.
- Audio restoration for imported recordings.

### 🤖 6. AI-Powered Songwriting Assistant

Use Google Gemini 2.5 Flash to develop and refine musical ideas.

- Generate song concepts from natural-language prompts.
- Create structured lyrics based on genre and mood.
- Suggest rhyming words and poetic expressions.
- Autocomplete lyrics while maintaining context.
- Analyze emotional progression and narrative coherence.
- Develop musical blueprints with suggested tempo, key, chord progressions, and song structure.

### ⚡ 7. Studio Workflow & Productivity

Work efficiently with global playback controls, keyboard shortcuts, and project history.

| Shortcut | Action |
|---|---|
| `Space` | Play or pause |
| `L` | Open Lyrics Studio |
| `M` | Open Mixer & Master |
| `C` | Open Music Composer & Piano Roll |
| `V` | Open Vocal Studio |
| `P` | Open Prompt & Song Generator |
| `Ctrl/Cmd + Z` | Undo |
| `Ctrl/Cmd + Shift + Z` | Redo |

**Export options include:**

- Standard MIDI files (`.mid`).
- Master WAV mixdowns.
- Individual audio stems.
- Lyric lead sheets.

## 🏗️ Architecture

Raag Studio uses a React-based frontend, a Web Audio API synthesis engine, and an Express backend that communicates with Google Gemini.

```text
Raag Studio
│
├── React 19 Frontend
│   ├── Prompt & Song Generator
│   ├── Lyrics Studio
│   ├── Music Composer & Piano Roll
│   ├── Harmonic Progression Studio
│   ├── Vocal Studio
│   ├── Audio Cleaner
│   ├── Mixer & Mastering Suite
│   └── Export Manager
│
├── Web Audio API Engine
│   ├── Procedural Instrument Synthesis
│   ├── Multitrack Sequencing
│   ├── Music Theory & Raga Engine
│   ├── Audio Effects Processing
│   └── MIDI Export
│
└── Express Backend
    ├── Song Idea Generation
    ├── Lyrics Generation
    ├── Rhyme Suggestions
    ├── Lyric Autocomplete
    └── Storyline Analysis
        │
        └── Google Gemini 2.5 Flash
```

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| React 19 | Frontend user interface |
| TypeScript | Type-safe application development |
| Vite | Development server and build tooling |
| Tailwind CSS v4 | Styling and responsive layouts |
| Motion | UI animations |
| Lucide React | Interface icons |
| Web Audio API | Procedural audio synthesis and effects |
| Canvas 2D API | Waveforms and audio visualization |
| Node.js | JavaScript runtime |
| Express | Backend API and server middleware |
| Google GenAI SDK | Gemini AI integration |
| Node.js Test Runner | Automated unit testing |

## 📁 Project Structure

```text
raag-studio/
├── index.html
├── metadata.json
├── package.json
├── server.ts
├── tsconfig.json
├── vite.config.ts
├── .env.example
│
└── src/
    ├── main.tsx
    ├── App.tsx
    ├── index.css
    │
    ├── audio/
    │   ├── engine.ts
    │   ├── musicTheory.ts
    │   ├── musicTheory.test.ts
    │   ├── dspCalculations.ts
    │   ├── dspCalculations.test.ts
    │   ├── rhymeDetection.ts
    │   ├── rhymeDetection.test.ts
    │   ├── meterAnalysis.ts
    │   ├── meterAnalysis.test.ts
    │   ├── sentimentAnalysis.ts
    │   └── storylineAnalysis.ts
    │
    └── components/
        ├── StudioHeader.tsx
        ├── PromptSection.tsx
        ├── LyricsStudio.tsx
        ├── StorylineSummaryPanel.tsx
        ├── MusicComposer.tsx
        ├── MelodicContourVisualizer.tsx
        ├── HarmonicProgressionStudio.tsx
        ├── VocalStudio.tsx
        ├── AudioCleaner.tsx
        ├── MixerAndMaster.tsx
        └── ExportModal.tsx
```

## 🚀 Getting Started

Follow these steps to run Raag Studio locally.

### Prerequisites

Make sure you have the following installed:

- **Node.js:** Version 20 or higher. Node.js 22 LTS is recommended.
- **npm:** Version 10 or higher.
- **Google Gemini API key:** Obtain one from [Google AI Studio](https://aistudio.google.com/).

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/raag-studio.git
cd raag-studio
```

Replace `your-username` with the actual GitHub username or organization hosting the repository.

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a local environment file from the example:

```bash
cp .env.example .env
```

On Windows Command Prompt, use:

```cmd
copy .env.example .env
```

Open `.env` and configure the following variables according to your server configuration:

```env
GEMINI_API_KEY=your-gemini-api-key-here
APP_URL=http://localhost:3000
PORT=3000
```

Replace the placeholder with your actual Gemini API key.

**Security note:** Keep your API key in the server-side environment. Never commit `.env` to Git or expose the key in frontend code.

### 4. Start the Development Server

```bash
npm run dev
```

Open your browser and navigate to:

[http://localhost:3000](http://localhost:3000)

If your Vite or Express configuration uses a different port, use the URL shown in your terminal.

## 🧪 Testing & Code Quality

Raag Studio includes unit tests for its core audio calculations, music theory, rhyme detection, syllable analysis, and storyline analysis.

Run the test suite:

```bash
npm run test
```

Run the project's configured lint or TypeScript verification command:

```bash
npm run lint
```

Build the application for production:

```bash
npm run build
```

The original project documentation reports 62 unit tests. Run the test suite locally to verify the current results.

## 📡 Backend API Reference

The Express backend exposes endpoints for AI-assisted songwriting and lyric analysis.

All endpoints use the `POST` method.

| Endpoint | Description |
|---|---|
| `/api/generate-song-idea` | Generates a song blueprint containing musical suggestions, structure, and lyrics. |
| `/api/generate-lyrics` | Generates lyrics based on creative prompts, rhyme schemes, and emotional direction. |
| `/api/suggest-rhymes` | Suggests rhyming words and poetic expressions. |
| `/api/suggest-lyrics-line` | Suggests the next lyric line based on context, rhyme, and meter. |
| `/api/analyze-storyline` | Analyzes emotional progression and narrative coherence across song sections. |

Requests are handled by the Express backend, which integrates with Google Gemini through the Google GenAI SDK.

The exact request and response schemas should be documented alongside the corresponding route implementations.

## 🎹 Supported Musical Scales

### Western Scales

- Major (Ionian)
- Natural Minor (Aeolian)
- Harmonic Minor
- Melodic Minor
- Dorian
- Phrygian
- Lydian
- Mixolydian
- Locrian
- Blues Minor
- Major Pentatonic
- Minor Pentatonic

### Indian Raga-Inspired Scales

- Bilawal
- Kalyan
- Khamaj
- Kafi
- Asavari
- Bhairav
- Bhairavi
- Todi
- Marwa
- Poorvi

*Note: These are the scale and raga-inspired options listed in the project documentation. A scale representation alone does not capture every aspect of a traditional raga's grammar, phrasing, and performance practice.*

## 🤝 Contributing

Contributions, suggestions, bug reports, and feature requests are welcome.

To contribute:

1. Fork the repository.
2. Create a feature branch.

   ```bash
   git checkout -b feature/amazing-feature
   ```

3. Make your changes and add appropriate tests.
4. Run the project's checks.

   ```bash
   npm run test
   npm run lint
   ```

5. Commit your changes.

   ```bash
   git commit -m "Add amazing feature"
   ```

6. Push your branch.

   ```bash
   git push origin feature/amazing-feature
   ```

7. Open a pull request describing your changes.

Please ensure your changes follow the existing code style and do not introduce regressions.

## 🗺️ Roadmap

Potential future enhancements include:

- [ ] Real-time vocal recording and processing improvements.
- [ ] Multilingual lyric generation.
- [ ] Additional instruments and synthesis models.
- [ ] Enhanced audio mixing and mastering.
- [ ] Collaborative music projects.
- [ ] Improved mobile and tablet experiences.
- [ ] Additional audio export formats.
- [ ] Expanded music theory and raga analysis.

This roadmap represents potential development directions, not a guarantee that these features are already implemented or scheduled.

## 🔐 Security & Responsible Use

- Keep API keys and other secrets out of source control.
- Validate and handle API requests securely.
- Respect copyright, licensing, and intellectual property rights.
- Obtain appropriate permission before using another person's voice or likeness.
- Review the applicable terms before distributing or commercially using AI-generated audio.
- Do not assume every generated song is automatically cleared for commercial use.

## 📄 License

This project is distributed under the **Apache License 2.0**.

See the [`LICENSE`](LICENSE) file for the complete license terms.

If the license file is missing from the repository, add the appropriate Apache 2.0 license text before describing the project as officially licensed under it.

---

<p align="center">
  🎵 <strong>Raag Studio — Turn Your Musical Ideas into Reality.</strong>
  <br />
  Built for musicians, producers, songwriters, and creative minds.
</p>
