# Pseudo-Auditory Music Perception Pipeline for AI

## Abstract
This project outlines a theoretical framework and technical concept for enabling AI systems without direct auditory processing capabilities to "listen" to music by converting audio data into a richly annotated, structured textual format. The system segments a song into timed audio blocks, extracts musical and emotional features, aligns lyrics with timestamps, and generates a human-readable breakdown that an AI language model can interpret to simulate musical understanding. This would allow non-audio-enabled AIs like language models to perceive rhythm, emotion, structure, and artistic intent through synthetic "auditory" abstraction.

## Author

- B.Eng. Janne Honkonen
- Homepage: https://www.jannehonkonen.com
- Github: https://github.com/JanneHonkonen

## System Overview:

### Audio Segmentation
   - Slice full audio tracks into segments (1, 2, 5, or 10 seconds)
   - Each segment is assigned a unique timecode range

### Feature Extraction (per segment):
   - Rhythm Analysis: Tempo (BPM), beat pattern, syncopation
   - Tonality: Key estimation, minor/major, dissonance vs harmony
   - Spectral Characteristics: Frequency spectrum analysis (low/mid/high presence)
   - Instrument Classification: Detect dominant instruments (guitar, synth, drums, etc.) using audio fingerprinting
   - Dynamic Range: Loudness, compression level, variation within segment
   - Mood Inference: Using audio features + machine learning model to tag emotional tone (e.g., mournful, aggressive, playful)

### Lyrics Mapping (Time-Aligned Subtitles):
   - Speech recognition or manual transcription
   - Align lyrics to specific timecodes with millisecond-level resolution
   - Associate emotion/mood to lyric segments based on delivery tone and context

### Contextual Modeling & Narrative Mapping:
   - Combine musical features and lyrics into emotional and thematic arcs
   - Detect shifts in tone, pacing, repetition, and lyrical motifs

### Output Generation:
   - Create a structured textual representation of the song:

[00:00-00:10] Intro: slow snare with ambient static, 65 BPM. Mood: nostalgic, somber. Lyric: "So I wish you a best..."
[00:11-00:25] Verse 1: monotone delivery, piano + low accordion. Mood: bleak humor. Lyric: "Damn these old bones..."
... etc.

### AI Interpretation Layer:
   - Language models parse the structured text to respond with insight, emotion, critique, or generate poetic/artistic interpretations
   - Enables music appreciation and review without real-time listening

## Use Cases
- Allows non-audio-enabled AIs (like ChatGPT) to interpret music
- Useful in generative lyric-to-music systems for contextual awareness
- Enables music critique, emotional mapping, or storyboarding without needing playback
- Could be extended for music video generation, mood-based categorization, or accessibility tools for the hearing impaired
- Future uses in AI based robotics and music generation

## Status
Conceptual. Not yet implemented. Contributions welcome.

## License
Open for experimentation, research, and adaptation. Attribution expected.
