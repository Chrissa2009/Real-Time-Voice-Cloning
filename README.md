# Real-Time-Voice-Cloning
This repository builds upon the original work by [CorentinJ’s Real-Time-Voice-Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning). Modifications and experiments were made to test alternative embedding architectures such as Transformers, CNNs, and LSTMs. All original credit for the voice cloning model and training pipeline goes to the original authors.

## Getting Started

### 🔧 Prerequisites

1. Install Python version **3.10.5**
2. Install PyTorch (follow the install instructions for your OS and CUDA version at [pytorch.org](https://pytorch.org/get-started/locally/))
3. Install all Python dependencies:

```bash
pip install -r requirements.txt
```

## 🏋️ Training

Run the following command to train the encoder:

```bash
python encoder_train.py <name-of-your-run> <full-path-to-clean_data_root> --no_visdom > output.txt

# for example: 
python encoder_train.py my_run "C:\Coding\DLProject\VCTK\encoder" --no_visdom > output.txt 2>&1
```

📝 Note: Make sure to change the name-of-your-run each time. Otherwise, it will resume training from the previous run checkpoint.

## 📄 Papers Implemented

| arXiv URL | Component | Title | Implementation Source |
|-----------|-----------|-------|------------------------|
| [1806.04558](https://arxiv.org/abs/1806.04558) | SV2TTS | Transfer Learning from Speaker Verification to Multispeaker Text-To-Speech Synthesis | This repo |
| [1802.08435](https://arxiv.org/abs/1802.08435) | WaveRNN (vocoder) | Efficient Neural Audio Synthesis | [fatchord/WaveRNN](https://github.com/fatchord/WaveRNN) |
| [1703.10135](https://arxiv.org/abs/1703.10135) | Tacotron (synthesizer) | Tacotron: Towards End-to-End Speech Synthesis | [fatchord/WaveRNN](https://github.com/fatchord/WaveRNN) |
| [1710.10467](https://arxiv.org/abs/1710.10467) | GE2E (encoder) | Generalized End-To-End Loss for Speaker Verification | This repo |
