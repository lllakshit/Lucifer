# 🔥 Project Lucifer 2.0

**A next-generation, voice-activated personal assistant designed to run locally on your PC.**  
Lucifer 2.0 is highly intelligent, deeply personalized, extensible, and built with privacy-first principles.

---

## 🧠 Overview

**Project Lucifer 2.0** is a self-contained, intelligent voice agent that augments your interaction with both your digital and physical environment. Unlike mainstream cloud-based assistants, **Lucifer 2.0** performs all core AI processing—understanding, reasoning, and response generation—**locally** on your machine.

It uses an internet connection for real-time information retrieval and smart device control, but **your personal data, voice, and learned behaviors never leave your computer**. The system continuously adapts to your unique usage, becoming a highly personalized assistant over time.

---

## ✨ Key Features

- **🎙️ Voice-Activated Interface**  
  Hands-free operation through a customizable wake word (default: `"Jarvis"` — feel free to change it to `"Lucifer"` or anything else).
  
- **🧬 Deep Personalization**  
  Built for a single user. Learns your voice, accent, and vocabulary for maximum accuracy.

- **📚 Continuous On-Device Learning**  
  Fine-tunes locally using your interaction data. No cloud training required.

- **🔌 Hybrid Online/Offline Processing**  
  Core logic runs locally. Internet is used only for fetching real-time data or external APIs/devices.

- **⚙️ Extensible Task Automation**  
  Control local apps, automate workflows, perform web queries, and interact with smart home devices (via Home Assistant, etc.).

- **🧩 Modular & Open Source**  
  Full control. Built using open-source components for transparency, hacking, and community-driven upgrades.

---

## 🏗️ Architecture & Tech Stack

Lucifer 2.0 is powered by a modular AI voice pipeline, all running on-device:

| Component             | Technology                          |
|----------------------|--------------------------------------|
| Wake Word Detection  | Lightweight custom trigger engine    |
| STT (Speech-to-Text) | [Whisper](https://github.com/openai/whisper) by OpenAI |
| NLU (Understanding)  | Local LLMs via [Ollama](https://ollama.com) / [GPT4All](https://gpt4all.io) |
| Dialogue Management  | [LangChain](https://www.langchain.com/) |
| TTS (Text-to-Speech) | [Bark](https://github.com/suno-ai/bark) for natural voice responses |
| Task Engine          | Native Python 3.8+ automation layer |

---

## 🖥️ System Requirements

### 💻 Recommended Hardware

- **OS:** Windows 11 or Ubuntu 22.04 LTS (64-bit)
- **CPU:** AMD Ryzen 7 / Intel Core i7 (multi-core)
- **GPU:** NVIDIA RTX series (6GB+ VRAM)
- **RAM:** 16 GB+
- **Storage:** 100+ GB free (for models, logs, cache)
- **Peripherals:** High-quality USB microphone

### 🧪 Minimum (CPU-only) Specs

- **CPU:** Modern quad-core
- **RAM:** 8–16 GB
- **Storage:** 100+ GB

---

## 🚀 Installation & Setup

> 📌 Detailed walkthroughs and automated setup scripts will be released with the first public alpha.

### Step 1: Clone the Repository

```bash
git clone https://github.com/[YourUsername]/Lucifer-2.0.git
cd Lucifer-2.0
```

### Step 2: Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Download AI Models

A `setup.sh` or `setup.bat` script will be provided to auto-download required STT, NLU, and TTS models.

### Step 5: Configure Lucifer

Edit the `config.yaml` file:

- Select microphone and speakers.
- Set API keys (if required).
- Choose your wake word.
- Customize output behavior.

### Step 6: Run Lucifer

```bash
python main.py
```

---

## 🌐 Future Scope

Lucifer's voice interface is just the beginning.

### Coming Soon:

- **🧠 BCI (Brain-Computer Interface) Integration**  
  Thought-to-command pipeline using real-time BCI signals.

- **📱 Mobile Companion App**  
  Secure syncing between your phone and PC, locally encrypted.

- **📡 LAN-Based Multi-Device Control**  
  Orchestrate IoT setups, PCs, displays, etc., over your local network.

---

## 🤝 Contributing

We welcome contributions from the open-source community!

Please read [`CONTRIBUTING.md`](CONTRIBUTING.md) for:

- 📋 Feature requests and bug reports  
- 🧪 Testing & improvements  
- 📘 Documentation updates  
- 🔧 Pull request standards

---

## 📄 License

Lucifer 2.0 is released under the **MIT License**. See the [`LICENSE`](LICENSE) file for details.

---

## 💬 Connect With Us

Stay tuned for:

- Discord community
- GitHub Discussions
- Weekly alpha build drops

---

> *“Privacy isn’t a feature. It’s your right. Lucifer is the voice of that freedom.”*
