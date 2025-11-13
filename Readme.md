<p align="center">
  <img src="https://blog.gensyn.ai/content/images/2025/11/CodeAssist-Blog.jpg" width="800" height="750" />
</p>

<h1 align="center">🚀 Gensyn CodeAssist — Local Setup Guide</h1>

---

# 🧠 What is CodeAssist?

**CodeAssist** is a fully local AI coding agent built by **Gensyn**.  
It runs entirely on your machine using **Docker + Ollama**, allowing you to:

### ✔ Features
- Write code  
- Debug code  
- Generate files  
- Ask coding questions  
- Build apps & scripts  
- Fully **private**, fully **local**, no cloud needed  
- Extremely lightweight & developer-friendly

---

# 🧩 Requirements

Before installing, ensure your system meets the following:

### ✔ Operating System
- Ubuntu 20.04 / 22.04  
- Linux  
- Windows (using WSL2)

### ✔ Hardware
- **8GB RAM minimum**, 16GB recommended  
- **10–20GB free disk space**  
- Internet required only during installation  
- Works **100% offline** after setup

### ✔ Software Needed
| Software | Version | Purpose |
|---------|---------|---------|
| **Docker** | Latest | Runs isolated containers |
| **Python3** | 3.8+ | UV runner |
| **pip3** | Latest | Python packages |
| **uv (Astral)** | Latest | Executes run.py |
| **Hugging Face Token** | Create new | Model downloads/uploads |

---

# ⚡ Installation Steps

Run these commands exactly in your Ubuntu terminal:

---

## **1️⃣ Update & upgrade your system**
```bash
sudo apt update && sudo apt upgrade -y
```

##  2️⃣ Install Docker + Enable Docker Service
```bash
sudo apt install docker.io -y
sudo systemctl enable docker
sudo service docker start
```

## 3️⃣ Check Docker Version
```bash
docker --version
```

## 4️⃣ Install Python 3 + PIP
```bash
sudo apt install python3 python3-pip -y
```

## 5️⃣ Verify Python & PIP
```bash
python3 --version
pip3 --version
```

## 6️⃣ Install UV Package Manager
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## 7️⃣ Verify UV Installation
```bash
uv --version
```

## 8️⃣ Clone CodeAssist Repository
```bash
git clone https://github.com/gensyn-ai/codeassist.git
cd codeassist

```

## 9️⃣ Start CodeAssist
```bash
uv run run.py
```

## 🔟 Enter Your HuggingFace Token
When prompted:
```bash
 HuggingFace token:
```
Paste your HF token and press Enter.








