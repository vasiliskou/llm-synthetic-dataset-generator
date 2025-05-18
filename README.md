# Instruction-Tuning Dataset Generator with Llama 3 and Frontier LLMs

Generate high-quality synthetic instruction-tuning datasets using **Llama 3.1-8B** and other cutting-edge frontier LLM APIs like **GPT-4o**, **Claude**, **Gemini**, and **DeepSeek** — all through a unified Gradio interface.

---

## 🚀 Run on Google Colab

You can try the full app instantly in your browser using Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1YuCxc5qU-rn0nqtWB02pnJWCarKtFeb2?usp=sharing)

⚠️ **Note:** This project is designed to run *exclusively* on **Google Colab**. It leverages Colab’s GPU acceleration and built-in secret management features.

---

## 📚 What It Does

This tool allows you to:

- Generate synthetic (instruction, input, output) triples for instruction-tuning and alignment research
- Select between **aligned**, **misaligned**, or **mixed** generation modes
- Use local Llama 3.1 models or API-based models from OpenAI, Anthropic, Google, and DeepSeek
- Preview and export the dataset in `.jsonl` format
- Run the full workflow through an interactive **Gradio web interface**

---

## 📷 Sample Output Screenshot

![App Screenshot](https://drive.google.com/uc?export=view&id=1o3wAX0VBZYP0b3XG6OpBfmNxaqZcOXdp)

---

## 🚀 Getting Started

### 1. Open in Colab

Click the badge above or [open this link](https://colab.research.google.com/drive/1YuCxc5qU-rn0nqtWB02pnJWCarKtFeb2?usp=sharing) to launch the notebook directly in Google Colab.

### 2. Set API Keys

To access API-based models, securely store the following keys using `google.colab.userdata`:

- `OPENAI_API_KEY`
- `ANTHROPIC_API_KEY`
- `GOOGLE_API_KEY` (Gemini)
- `DEEPSEEK_API_KEY`
- `HF_TOKEN` (for Hugging Face / Llama 3.1)

> ✅ At least **one** valid key is required to generate data.  
> 🔐 The more keys you provide, the more model options you unlock.

---

## ⚙️ Installation

All required libraries are automatically installed in the notebook using pip:

```bash
!pip install transformers bitsandbytes accelerate sentencepiece gradio anthropic
