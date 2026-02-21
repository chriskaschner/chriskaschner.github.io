---
title: "vegF1"
date: 2026-02-09
summary: "F1 video profanity replacement — swear words become vegetables via AI speech synthesis"
tags: ["python", "ai", "whisperx", "tts"]
weight: 2
---

Automatically replaces profanity in Formula 1 videos with vegetable names using AI speech synthesis.

Inspired by a Missed Apex podcast joke: *"Surely AI can replace the words with random fruits and vegetables."*

**Example replacements:**

| Original | Output |
|----------|--------|
| "What the fuck?" | "What the butternut squash?" |
| "fucking blind asshole" | "broccoli... blind... kale" |
| "fucking motherfucker" | "bamboo shoots, fenugreek, chard" |
| "fucking dickhead" | "collard greens, garlic" |
| "fuck sake" | "rhubarb sake" |

Non-swear words are preserved — only the profanity gets replaced.

**How it works:**
- WhisperX provides word-level transcription with timestamps
- TTS generates matching vegetable name audio clips
- Timeline-based architecture handles phrase detection, word-level replacement with 400ms buffers, and multiple vegetable fills
- 95%+ duration matching so it sounds natural
- 0 swear words in output (verified by re-transcription)

**Tech:** Python, WhisperX, TTS, FFmpeg

[Source on GitHub](https://github.com/chriskaschner/vegF1)
