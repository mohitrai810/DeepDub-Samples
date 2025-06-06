# DeepDub : A video dubbing platform  [Link ](https://huggingface.co/spaces/mohitrai76/DeepDub)

This repository showcases sample outputs of **DeepDub**, a multilingual video dubbing system that translates and synthesizes speech in different languages while preserving the original tone .

Here are some samples

## Original Video

- [OriginalSample.mp4](./OriginalSample.mp4)

## Translated Samples

Below are the translated versions of the original video in multiple languages:

- [SampleEnglish.mp4](./SampleEnglish.mp4)
- [SampleHindi.mp4](./SampleHindi.mp4)
- [SampleFrench.mp4](./SampleFrench.mp4)
- [SampleSpanish.mp4](./SampleSpanish.mp4)

## About the Project

**DeepDub** is a dubbing pipeline that combines the following components:

- **Transcription**: Speech-to-text using [WhisperX](https://github.com/m-bain/whisperx)
- **Translation**: Language translation via [OpenRouter API](https://openrouter.ai/)
- **Emotion Detection**: Analyzes emotional tone for expressive synthesis
- **Text-to-Speech**: Uses [edge TTS](https://github.com/rany2/edge-tts) for voice generation with tonal variation
- **Alignment**: Time-synchronized audio using `pyrubberband`

This enables multilingual dubbing that is both accurate and expressive.

## How It Works

1. Transcribe the original video using WhisperX
2. Translate the text into the target language
3. Detect emotions in speech
4. Generate emotional speech using XTTSv2
5. Adjust timing to match original video duration
6. Merge dubbed audio with the original video
