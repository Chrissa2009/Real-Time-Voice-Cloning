# Real-Time-Voice-Cloning
This repository builds upon the original work by [CorentinJ’s Real-Time-Voice-Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning). Modifications and experiments were made to test alternative embedding architectures such as Transformers, CNNs, and LSTMs. All original credit for the voice cloning model and training pipeline goes to the original authors.

## Papers Implemented

| arXiv URL | Component | Title | Implementation Source |
|-----------|-----------|-------|------------------------|
| [1806.04558](https://arxiv.org/abs/1806.04558) | SV2TTS | Transfer Learning from Speaker Verification to Multispeaker Text-To-Speech Synthesis | This repo |
| [1802.08435](https://arxiv.org/abs/1802.08435) | WaveRNN (vocoder) | Efficient Neural Audio Synthesis | [fatchord/WaveRNN](https://github.com/fatchord/WaveRNN) |
| [1703.10135](https://arxiv.org/abs/1703.10135) | Tacotron (synthesizer) | Tacotron: Towards End-to-End Speech Synthesis | [fatchord/WaveRNN](https://github.com/fatchord/WaveRNN) |
| [1710.10467](https://arxiv.org/abs/1710.10467) | GE2E (encoder) | Generalized End-To-End Loss for Speaker Verification | This repo |
