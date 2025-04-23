# Speech-Enhancement-Using-UNet-Architecture

## 🎧 Speech Enhancement Using U-Net

Enhance speech clarity by removing background noise using a U-Net-based deep learning model. Built with **clean and efficient Python tools**—no `librosa`, just `scipy`, `numpy`, and `soundfile`. Ideal for speech applications in **assistive tech**, **telephony**, and **AI voice agents**.

---

### 🌟 Features

- 🧠 **U-Net architecture** tailored for spectrogram denoising  
- 🔊 **Soundfile-based audio pipeline** — lightweight and modern  
- 📈 Spectrogram-based processing with STFT/ISTFT  
- 🎧 Supports real-world datasets like:
  - [LibriSpeech](https://www.openslr.org/12) (clean speech)
  - [ESC-50](https://github.com/karoldvl/ESC-50) (environmental noise)
- 🧪 Training and prediction from scratch or with pre-trained models

---

### 📁 Project Structure

```
SpeechEnhancementUsingUNet/
├── data_tools.py            # Audio preprocessing, framing, and STFT/ISTFT
├── model.py                 # Custom U-Net model
├── train.py                 # Model training loop
├── prediction_denoise.py    # Denoising and inference logic
├── main.py                  # Run training or inference
├── samples/                 # Audio samples (noisy/clean/denoised)
└── SpeechEnhancementUsingUNet.ipynb  # Interactive notebook demo
```

---

### ⚙️ Setup

```bash
git clone https://github.com/yourusername/SpeechEnhancementUsingUNet.git
cd SpeechEnhancementUsingUNet
pip install -r requirements.txt
```

---

### 🚀 Train the Model

```bash
python main.py --mode train --epochs 50 --batch_size 16
```

Customize with:
- `--frame_length`
- `--hop_length`
- `--sample_rate`
- `--dim_spectrogram`

---

### 🔮 Denoise Audio

```bash
python main.py --mode predict --weights_path ./checkpoints/model.h5 --input_audio ./samples/noisy.wav
```

The cleaned output will be saved under `./predictions/`.

---

### 📊 Datasets Used

- **[LibriSpeech](https://www.openslr.org/12)** — Clean speech for supervised learning  
- **[ESC-50](https://github.com/karoldvl/ESC-50)** — Realistic noise conditions

You can also use your own WAV files!

---

### 📌 Highlights

- 🚫 **No Librosa** — 100% compatible with `scipy`, `soundfile`, and `numpy`
- 🎯 Scalable spectrogram learning via STFT
- 💡 Built for academic research and production experimentation

---

### 👤 Contact

For questions, collaboration, or feedback:  
📧 **sanyashresta@gmail.com**

---

### 📜 License

MIT License — use, modify, and share freely.

---

Let me know if you want to include:  
- A table of audio examples  
- Training logs or learning curve visualizations  
- Streamlit or Gradio demo setup
