
# 🎙️ AI Voice Cloning Studio

> **Create multilingual, high-quality speech from any voice sample. Featuring live recording, noise reduction, and expressive cloning powered by state-of-the-art TTS models.**

---

## 🚀 Overview

**AI Voice Cloning Studio** is an interactive Jupyter-based application that enables users to:

* Upload or record a **voice sample**
* Input **custom text**
* Select from multiple **languages**
* Generate a **natural-sounding voice clone**
* Apply **audio enhancement** for improved clarity

It combines the power of [Coqui TTS](https://github.com/coqui-ai/TTS) and custom DSP with an intuitive UI built using `ipywidgets`.

---

## ✨ Key Features

| Feature                          | Description                                                                   |
| -------------------------------- | ----------------------------------------------------------------------------- |
| 🔊 **Voice Cloning**             | Generate speech using a reference speaker’s voice                             |
| 🌐 **Multilingual**              | Supports cloning in English, Spanish, French, German, Italian, and Portuguese |
| 🎙 **Live Microphone Recording** | Record your own voice sample directly within the interface                    |
| 🧹 **Noise Reduction**           | High-pass filtering to remove background noise                                |
| 🧠 **XTTS v2 Integration**       | Leverages Coqui’s zero-shot multilingual cloning                              |
| 🎛️ **Enhanced UI**              | Modern interface with responsive design and user feedback                     |

---

## 📸 Interface Preview

<p align="center">
  <img width="852" height="302" alt="pic 1" src="https://github.com/user-attachments/assets/d703920a-a018-49c3-967b-eaa3e65c7706" />
  <img width="857" height="302" alt="pic 2" src="https://github.com/user-attachments/assets/2401efbb-1ba5-40b6-ad40-9c803ff087fb" />
  <img width="860" height="302" alt="pic3" src="https://github.com/user-attachments/assets/c6d28cb7-3935-4e47-8906-0674505a61a3" />

  <img width="867" height="302" alt="pic 4" src="https://github.com/user-attachments/assets/ff9fd763-ab93-4fd2-97e4-ff5f26636ad0" />



</p>

---

## 🛠️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/voice-cloning-studio.git
cd voice-cloning-studio
```

### 2. Set Up Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Launch the Application

```bash
jupyter notebook voice_cloning_studio.ipynb
```

> ✅ For JupyterLab: `jupyter lab` (ensure `jupyter-widgets/jupyterlab-manager` is installed)

---

## 🧪 Dependencies

Minimal `requirements.txt`:

```
torch>=1.12.0
TTS>=0.17.3
ipywidgets
sounddevice
scipy
numpy
```

You can install them manually or with:

```bash
pip install torch TTS ipywidgets sounddevice scipy numpy
```

---

## 🌍 Supported Languages

| Language   | Code |
| ---------- | ---- |
| English    | en   |
| Spanish    | es   |
| French     | fr   |
| German     | de   |
| Italian    | it   |
| Portuguese | pt   |

---

## 📂 File Structure

```
voice-cloning-studio/
├─ voice sample                # for  testing
├── voice_cloning_studio.ipynb # Main Jupyter interface
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
└── LICENSE                     # MIT license
```

---

## 🧠 Under the Hood

* **TTS Model**: [`tts_models/multilingual/multi-dataset/xtts_v2`](https://github.com/coqui-ai/TTS)
* **Audio Preprocessing**:

  * Stereo to mono conversion
  * Normalization
  * High-pass filtering (cutoff at 100Hz)
* **UI Framework**: `ipywidgets`, styled with custom CSS
* **Voice Input Options**: Microphone or upload (`.wav`, `.mp3`, `.ogg`)

---

## 📝 Usage Workflow

1. **Upload** a voice sample or **record live**
2. Enter the **text** to be spoken
3. Select a **language**
4. Click **“Generate Voice Clone”**
5. Listen to and **download** your enhanced cloned voice

---

## ✅ Sample Output

<p align="center">
  <img width="796" height="302" alt="pic 6" src="https://github.com/user-attachments/assets/248ecd94-6a9f-4047-96a4-c60f195f7ba5" />
  <img width="852" height="302" alt="5" src="https://github.com/user-attachments/assets/a1237fcf-b2cb-4a66-823b-71f0d43e67d7" />

 
</p>

---

## 🧑‍💻 Author

**Muhammad Zuhaib**
GitHub: https://github.com/Zuhaib23

---

## 📄 License

This project is licensed under the **MIT License**.
See the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgments

* [Coqui TTS](https://github.com/coqui-ai/TTS)
* [Jupyter Widgets](https://github.com/jupyter-widgets/ipywidgets)
* [SciPy](https://scipy.org/)
* [NumPy](https://numpy.org/)
* [Python SoundDevice](https://python-sounddevice.readthedocs.io/)

---

## ⭐ Show Your Support

If you find this project useful, consider starring 🌟 the repository and sharing it with others!

---

