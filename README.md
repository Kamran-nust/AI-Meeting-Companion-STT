# AI Meeting Companion - STT

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Transformers](https://img.shields.io/badge/🤗_Transformers-4.36.0-orange.svg)](https://huggingface.co/docs/transformers/index)
[![Gradio](https://img.shields.io/badge/Gradio-5.23.2-green.svg)](https://gradio.app/)

An AI-powered meeting companion that transcribes speech to text and analyzes meeting content using advanced language models. Built with OpenAI's Whisper, IBM Watson, and Meta's Llama models.

## 🚀 Features

- **Speech-to-Text Transcription**: High-accuracy audio transcription using OpenAI's Whisper model
- **Web Interface**: User-friendly Gradio interface for easy audio file uploads
- **Meeting Analysis**: Extract key points and insights from transcribed meetings using LLMs
- **Multiple Models**: Support for both simple transcription and advanced analysis
- **Real-time Processing**: Efficient batch processing for long audio files

## 📋 Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## 🛠 Installation

### Prerequisites

- Python 3.8 or higher
- FFmpeg (for audio processing)

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Kamran-nust/AI-Meeting-Companion-STT.git
   cd AI-Meeting-Companion-STT
   ```

2. **Create a virtual environment:**
   ```bash
   pip3 install virtualenv
   virtualenv my_env
   source my_env/bin/activate  # On Windows: my_env\Scripts\activate
   ```

3. **Install required packages:**
   ```bash
   pip install transformers==4.36.0 torch==2.1.1 gradio==5.23.2 langchain==0.0.343 ibm_watson_machine_learning==1.0.335 huggingface-hub==0.28.1
   ```

4. **Install FFmpeg:**
   ```bash
   sudo apt update
   sudo apt install ffmpeg -y
   ```

## 🎯 Usage

### Simple Speech-to-Text

Run the basic transcription script:

```bash
python simple_speech2text.py
```

### Web Application

Launch the Gradio web interface:

```bash
python speech2text_app.py
```

Then open your browser to `http://localhost:7860` to upload audio files and get transcriptions.

### Advanced Meeting Analysis

For meeting analysis with key point extraction:

```bash
python speech_analyzer.py
```

## 📋 Requirements

- `transformers==4.36.0` - Hugging Face Transformers library
- `torch==2.1.1` - PyTorch for model inference
- `gradio==5.23.2` - Web interface framework
- `langchain==0.0.343` - LLM framework integration
- `ibm_watson_machine_learning==1.0.335` - IBM Watson integration
- `huggingface-hub==0.28.1` - Hugging Face Hub client
- `ffmpeg` - Audio processing library

## 📁 Project Structure

```
AI-Meeting-Companion-STT/
├── README.md                    # Project documentation
├── hello.py                     # Simple test script
├── simple_speech2text.py        # Basic speech-to-text transcription
├── speech2text_app.py          # Gradio web application
├── speech_analyzer.py          # Advanced meeting analysis
└── simple_llm/                 # LLM-related utilities
```

## 🙏 Acknowledgments

- OpenAI for the Whisper model
- Hugging Face for the Transformers library
- IBM Watson for language model integration
- Meta for the Llama models
- The Gradio team for the web interface framework

---

This is part of IBM GenAI specialization course project

