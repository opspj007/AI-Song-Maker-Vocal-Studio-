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


Here is the complete file content:
code

# 🎵 AI Song Maker & Vocal Studio (Raag Studio)

> **Next-generation, browser-based AI music production workstation, vocal studio, and songwriting companion powered by Google Gemini 2.5 Flash, Web Audio API DSP synthesis, and real-time multitrack sequencing.**

[![TypeScript](https://img.shields.io/badge/TypeScript-5.x%20%7C%207.x-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React 19](https://img.shields.io/badge/React-19.0-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![Vite 8](https://img.shields.io/badge/Vite-8.3-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS v4](https://img.shields.io/badge/Tailwind-v4.3-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio%20API-DSP%20Synthesis-FF5722)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Gemini 2.5 Flash](https://img.shields.io/badge/Google%20Gemini-2.5%20Flash-8E75B2?logo=google)](https://ai.google.dev/)
[![Tests Passing](https://img.shields.io/badge/Tests-62%20passed-22c55e?logo=node.js)](https://nodejs.org/)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

---

## 🌟 Overview

**AI Song Maker & Vocal Studio** is a full-stack digital audio workstation (DAW) and lyric-composition laboratory designed right in the browser. It combines algorithmic Indian classical and Western music theory engines, real-time Web Audio API procedural sound synthesis (featuring Harmonium, Bansuri, Sitar, Tanpura, Dholak, and 808 Sub-bass), an intelligent lyric-writing suite with phonetic rhyme detection and narrative arc analysis, alongside AI assistance powered by **Google Gemini 2.5 Flash**.

Whether you are crafting Bollywood romantic ballads, high-energy Punjabi pop, Sufi qawwali, lo-fi chillhop, or contemporary cinematic scores, this studio gives you end-to-end creative control from initial prompt to mastered stem export.

---

## 🚀 Key Features

### 1. 🎛️ Multitrack Web Audio DSP Synthesizer & Piano Roll
- **Zero External Audio File Latency**: 100% client-side DSP synthesis using Web Audio API nodes (`OscillatorNode`, `BiquadFilterNode`, `GainNode`, `ConvolverNode`, `WaveShaperNode`).
- **Authentic World & Indian Classical Instruments**:
  - **Sitar**: Resonant sympathetic buzz with physical pluck modeling.
  - **Bansuri (Bamboo Flute)**: Breathy sine-wave synthesis with authentic subtle pitch vibrato.
  - **Harmonium**: Rich dual-reed warm detuned sawtooth synthesis with swell dynamics.
  - **Tanpura**: Continuous multi-string drone bed with overtone shimmer.
  - **Dholak / Tabla**: Procedural percussion modeling resonant bass *bayan* slaps and high *dayan* snaps.
  - **Sub Bassline / 808**: Punchy sine-wave sub with soft-clipping saturation.
- **Interactive MIDI Piano Roll**:
  - Visual note grid mapping octaves C2 through B5.
  - Click-to-add, click-to-delete, drag-and-resize note duration.
  - Octave switching, zoom controls, and live playback cursor synchronization.
  - High-precision export to standard `.mid` (MIDI Type 0/1) files.

### 2. ✍️ Lyric Studio & Rhyme Intelligence Engine
- **Phonetic Rhyme Detection**: Analyzes end rhymes across lines, categorizing them into Perfect, Family, Assonance, and Radif/Qafia (Urdu/Hindi poetic meters).
- **Rhyme Scheme Recognition**: Automatically calculates pattern detection (AABB, ABAB, AAAA, Ghazal Radif/Qafia).
- **Syllable & Meter Counter**: Real-time syllable stress breakdown to ensure melodic rhythm balance.
- **Emotional Storyline Arc Analyzer**: Evaluates narrative progression across Verse 1, Verse 2, Chorus, and Bridge, graphing emotional valence and narrative coherence.
- **AI-Powered Rhyme Auto-Complete**:
  - Context-aware lyric suggestions driven by Gemini 2.5 Flash.
  - Suggests the next rhyming line respecting current mood, genre, and phonetic rhyme scheme.
  - One-click insertion directly into the lyrics editor.

### 3. 🎼 Harmonic Progression Studio & Raga Modes
- **Modal Interchange & Scales**: Support for Western Major/Minor, Dorian, Phrygian, Mixolydian, as well as Indian Classical That/Raag scales (Bilawal, Kafi, Bhairav, Yaman, Kalyan, Khamaj, Asavari, Todi, Marwa).
- **Chord Progression Generator**: Interactive chord pads with real-time audio auditioning.
- **Melodic Contour Visualizer**: Canvas-based real-time rendering of pitch curves, melodic transitions, and interval dynamics.

### 4. 🎚️ Multitrack Mixer & Mastering Suite
- **Channel Strips**: Individual faders with dB gain metering, stereo panning, solo, and mute states.
- **Master Effects Chain**:
  - 3-Band Parametric EQ (Low shelf, Mid peak, High shelf).
  - Studio Compressor (Threshold, Ratio, Attack, Release).
  - Algorithmic Space Reverb & Tape Delay.
  - Master Limiter and Soft-clipping Maximizer.
- **Real-Time Oscilloscope & Waveform Canvas**:
  - Live audio spectrum analyzer and time-domain oscilloscope rendered at 60 FPS on HTML5 Canvas.

### 5. 🧹 Audio Cleaner & AI Vocal Production Studio
- **Vocal Processing Chain**: Formant pitch-correction / auto-tune engine, de-esser, vocal warmth saturation, and doubler/chorus effect.
- **Audio Restoration**: Background denoiser, room hum suppressor, and transient shaper for imported voice memos or live microphone recordings.

### 6. ⚡ Studio Workflow & Productivity
- **Global Studio Keyboard Shortcuts**:
  - <kbd>Space</kbd>: Global Play / Pause toggle.
  - <kbd>L</kbd>: Jump instantly to **Lyrics Studio**.
  - <kbd>M</kbd>: Jump instantly to **Mixer & Master**.
  - <kbd>C</kbd>: Jump to **Music Composer & Piano Roll**.
  - <kbd>V</kbd>: Jump to **Vocal Studio**.
  - <kbd>P</kbd>: Jump to **Prompt & Song Generator**.
  - <kbd>Ctrl</kbd> + <kbd>Z</kbd> / <kbd>Cmd</kbd> + <kbd>Z</kbd>: Undo project changes.
  - <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Z</kbd> / <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>Z</kbd>: Redo project changes.
- **Deep Undo / Redo History Stack**: Full immutable project snapshot history covering lyrics, arrangement blocks, stem volumes, and tempo changes.
- **Export Formats**: Standard MIDI file (`.mid`), master WAV mixdown, individual stem tracks, and lyric lead-sheet export.

---

## 🏗️ Architecture & Tech Stack
┌─────────────────────────────────────────────────────────────┐
│ React 19 SPA │
│ ┌───────────────┐ ┌────────────────┐ ┌──────────────────┐ │
│ │ PromptSection │ │ LyricsStudio │ │ MusicComposer │ │
│ │ (Song Gen) │ │ (Rhyme Engine)│ │ (MIDI Roll) │ │
│ └───────┬───────┘ └────────┬───────┘ └────────┬─────────┘ │
│ │ │ │ │
│ ┌───────┴───────┐ ┌────────┴───────┐ ┌────────┴─────────┐ │
│ │ VocalStudio │ │ MixerMaster │ │ StudioShortcuts │ │
│ │ (Pitch/Tune) │ │ (DSP FX Rack) │ │ (Global Hotkeys) │ │
│ └───────┬───────┘ └────────┬───────┘ └────────┬─────────┘ │
│ │ │ │ │
│ ▼ ▼ ▼ │
│ ┌───────────────────────────────────────────────────────┐ │
│ │ Web Audio DSP Engine (engine.ts) │ │
│ │ - Polyphonic Synth - Sitar / Bansuri / Harmonium │ │
│ │ - Dholak / Tabla - Tanpura Drone - Master Bus │ │
│ └──────────────────────────┬────────────────────────────┘ │
└─────────────────────────────┼───────────────────────────────┘
│ HTTP / REST
▼
┌─────────────────────────────────────────────────────────────┐
│ Express Backend (server.ts) │
│ ┌───────────────────────────────────────────────────────┐ │
│ │ POST /api/generate-song-idea │ │
│ │ POST /api/generate-lyrics │ │
│ │ POST /api/suggest-rhymes │ │
│ │ POST /api/suggest-lyrics-line (AI Autocomplete) │ │
│ │ POST /api/analyze-storyline │ │
│ └──────────────────────────┬────────────────────────────┘ │
│ │ Google GenAI SDK │
│ ▼ │
│ Google Gemini 2.5 Flash API │
└─────────────────────────────────────────────────────────────┘
code
Code
### Technology Highlights
- **Frontend**: [React 19](https://react.dev/), [TypeScript](https://www.typescriptlang.org/), [Tailwind CSS v4](https://tailwindcss.com/), [Motion (Framer Motion)](https://motion.dev/), [Lucide React](https://lucide.dev/).
- **Audio & Signal Processing**: Native Web Audio API, Canvas 2D API for 60fps waveforms and spectrograms.
- **Backend / Dev Server**: [Express](https://expressjs.com/) with [Vite](https://vitejs.dev/) middleware and [tsx](https://github.com/privatenumber/tsx).
- **Artificial Intelligence**: `@google/genai` with model `gemini-2.5-flash`.
- **Testing**: Built-in Node.js Test Runner (`node --test` / `tsx --test`) with 62 unit tests validating DSP calculations, rhyme phonetics, syllable meter, musical scales, and storyline sentiment.

---

## 📁 Repository Structure
.
├── index.html # App entry point with meta tags & Google fonts
├── metadata.json # AI Studio applet configuration & permissions
├── package.json # Project dependencies, scripts, and engine specs
├── server.ts # Full-stack Express server + Gemini AI endpoints + Vite middleware
├── tsconfig.json # TypeScript compiler configuration
├── vite.config.ts # Vite 8 configuration with Tailwind CSS v4 & React plugin
├── .env.example # Example environment variables template
│
└── src/
├── main.tsx # React root mount
├── App.tsx # Primary state coordinator, hotkeys, undo/redo, transport
├── index.css # Tailwind v4 theme configuration & audio canvas styling
│
├── audio/ # Audio core, music theory & analysis engines
│ ├── engine.ts # Web Audio API procedural synthesizer, stems, MIDI export
│ ├── musicTheory.ts # Ragas, scales, chord progressions, Roman numeral analysis
│ ├── musicTheory.test.ts # Music theory unit tests (14 tests)
│ ├── dspCalculations.ts # Gain-to-dB, EQ filters, compressor curve calculations
│ ├── dspCalculations.test.ts # DSP unit tests (10 tests)
│ ├── rhymeDetection.ts # Phonetic rhyme matcher, CMU-style phoneme scoring, Ghazal meter
│ ├── rhymeDetection.test.ts # Rhyme engine tests (13 tests)
│ ├── meterAnalysis.ts # Syllable counter, rhythmic stress parser
│ ├── meterAnalysis.test.ts # Meter unit tests (10 tests)
│ ├── sentimentAnalysis.ts # Lexical valence, emotional tone analyzer
│ ├── sentimentAnalysis.test.ts # Sentiment unit tests (8 tests)
│ ├── storylineAnalysis.ts # Song narrative arc evaluator (Verse -> Chorus -> Outro)
│ └── storylineAnalysis.test.ts # Storyline arc tests (7 tests)
│
└── components/ # Modular UI views & audio controls
├── StudioHeader.tsx # Global playback transport, BPM, key, undo/redo buttons
├── PromptSection.tsx # AI prompt-to-song blueprint generator
├── LyricsStudio.tsx # Interactive lyric editor with live rhyme & meter stats
├── StorylineSummaryPanel.tsx # Visual narrative arc, valence graph & lyrical coaching
├── MusicComposer.tsx # MIDI Piano Roll editor, track selector & scale picker
├── MelodicContourVisualizer.tsx # Real-time pitch contour & melody canvas
├── HarmonicProgressionStudio.tsx# Modal interchange, chord pads & raga progression studio
├── VocalStudio.tsx # Vocal tuner, formant pitch-shifter, live mic monitor
├── AudioCleaner.tsx # Noise gate, hum remover & audio restorer
├── MixerAndMaster.tsx # Multitrack mixer, faders, pan, master FX rack & oscilloscope
└── ExportModal.tsx # Stem export, WAV mixdown, and MIDI file downloader
code
Code
---

## 🛠️ Getting Started

### Prerequisites
- **Node.js**: `v20.0.0` or higher (Node 22 LTS recommended)
- **npm**: `v10.0.0` or higher
- **Google Gemini API Key**: Obtainable for free at [Google AI Studio](https://aistudio.google.com/).

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/raag-studio.git
   cd raag-studio
Install dependencies:
code
Bash
npm install
Configure Environment Variables:
Copy .env.example to .env:
code
Bash
cp .env.example .env
Open .env and add your Gemini API key:
code
Env
GEMINI_API_KEY="your-gemini-api-key-here"
APP_URL="http://localhost:3000"
PORT=3000
Launch the Development Server:
code
Bash
npm run dev
Open your browser and navigate to http://localhost:3000.
🧪 Testing & Code Quality
The project includes a comprehensive suite of 62 unit tests verifying core math, music theory algorithms, DSP curves, and phonetic analysis.
Run all tests:
code
Bash
npm run test
Run TypeScript verification:
code
Bash
npm run lint
Build for production:
code
Bash
npm run build
📡 Backend API Reference
All AI endpoints are proxied securely through server.ts to protect your API keys.
Endpoint	Method	Description
/api/generate-song-idea	POST	Generates a complete song structure (genre, tempo, key, raga, chord progression, and full lyrics) from a natural language prompt.
/api/generate-lyrics	POST	Crafts multi-verse lyrics adhering to specific rhyme schemes (e.g., Ghazal, Pop AABB) and emotions.
/api/suggest-rhymes	POST	Returns a list of categorized rhyming words and poetic metaphors for a given word and language context.
/api/suggest-lyrics-line	POST	Suggests the immediate next rhyming line based on prior lines, meter balance, and current emotion.
/api/analyze-storyline	POST	Evaluates the emotional arc and narrative coherence of the lyrics across song sections.
🎹 Supported Scales & Ragas
Category	Available Modes
Western Scales	Major (Ionian), Natural Minor (Aeolian), Harmonic Minor, Melodic Minor, Dorian, Phrygian, Lydian, Mixolydian, Locrian, Blues Minor, Major Pentatonic, Minor Pentatonic
Indian Raga Scales (Thaats)	Bilawal (Major), Kalyan (Lydian), Khamaj (Mixolydian), Kafi (Dorian), Asavari (Natural Minor), Bhairav (Double Harmonic), Bhairavi (Phrygian), Todi, Marwa, Poorvi
🤝 Contributing
Contributions are welcome! Please feel free to open an issue or submit a pull request.
Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Ensure all tests pass (npm run test && npm run lint)
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
📄 License
Distributed under the Apache License 2.0. See LICENSE for more information.
<p align="center">
Crafted with ❤️ for musicians, producers, and songwriters worldwide.
</p>
```
