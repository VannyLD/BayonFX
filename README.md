# 🎬 BayonFX Pro

**Advanced AI Video Editor Studio**

BayonFX Pro is a high-performance desktop application built with Python and PySide6. Designed specifically for content creators, it bridges the gap between AI text-to-speech generation, precise subtitle synchronization, and rapid video exporting. 

Featuring full 100% Khmer language support, offline AI voice models, and direct CapCut draft integration, BayonFX drastically reduces the time it takes to produce professional, dubbed social media content.

---

## ✨ Key Features

* 🗣️ **Hybrid AI Voice Generation:** * Seamlessly generate AI voiceovers using Google TTS, Edge TTS, and **fully offline Khmer MMS TTS** via PyTorch.
  * Apply custom DSP audio effects (Pitch, Speed, Studio Reverb, Bass/Treble Enhancer) directly via FFmpeg.
* ✂️ **Interactive Timeline Studio:** * A custom-built PySide6 timeline allowing users to drag, drop, and trim subtitle and audio blocks perfectly in sync with the video proxy preview.
* 🚀 **Direct CapCut Export Engine:** * Bypass standard rendering completely. BayonFX can compile your video, AI audio, subtitles, and PIP logos directly into a native CapCut Draft folder (`draft_content.json`), ready for final tweaks.
* 🔥 **Hardware-Accelerated Rendering:** * When hard-rendering is required, the app leverages FFmpeg with native GPU acceleration (NVIDIA NVENC, AMD AMF, Intel QSV) for blazing-fast export times.
* 📝 **Advanced Subtitle Engine:** * Parse, edit, and hard-burn `.srt` files into the video using `pysubs2` and ASS subtitle formatting. Supports custom fonts (Khmer OS Siemreap), colors, and background opacity.
* 🛡️ **Secure Machine Licensing:** * Built-in hardware ID generation and online JSON license verification to protect the software.

---

## 🛠️ Tech Stack

BayonFX is powered by a robust Python ecosystem:
* **UI Framework:** PySide6 (Qt for Python)
* **Video/Audio Processing:** FFmpeg, OpenCV (`cv2`), `moviepy`, `pydub`
* **AI & Machine Learning:** PyTorch, Transformers (HuggingFace), OpenAI Whisper
* **Subtitle Processing:** `pysubs2`
* **System OS:** Designed for Windows (compiled via PyInstaller)

---

## 📂 Project Architecture

The application is structured into modular classes for maintainability:
* `Main.py`: The core application entry point and licensing engine.
* `voice_premium.py`: The advanced AI timeline, CapCut JSON builder, and FFmpeg render engine.
* `Subtitles_Class.py` / `SRT_Class.py`: Handlers for text parsing and translation.
* `ui_bayonfx.py` / `ui_prevoice.py`: Compiled Qt Designer UI files.

---
