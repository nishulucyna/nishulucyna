<h1 align="center">Hi, I'm Anish 👋</h1>
<p align="center">
  <a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white"></a>
  <a href="https://linkedin.com/in/YOUR_LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white"></a>
</p>

## 🔐 Post-Quantum Hybrid Encryption (Techfest, 1st Year)

A hybrid Post-Quantum Cryptographic communication model combining classical symmetric encryption with NIST-standardized quantum-resistant algorithms — built to defend against "harvest now, decrypt later" attacks.

- **Key exchange:** ML-KEM / CRYSTALS-Kyber for quantum-resistant key encapsulation.
- **Signatures:** ML-DSA / CRYSTALS-Dilithium for origin authentication and non-repudiation.
- **Bulk encryption:** AES-256-GCM, with the session key derived from the Kyber shared secret via KDF.
- Full sender→receiver pipeline: encapsulation → key derivation → AES-GCM encryption → Dilithium signing → verification → decapsulation → decryption.
- **Identified an unresolved trust-bootstrapping limitation:** explored using a QRNG-based commitment scheme to remove the need for out-of-band key exchange, and demonstrated that commitment alone doesn't authenticate origin — a MITM can still substitute commitments before any channel is authenticated. This confirmed that hybrid PQC pipelines still require an authenticated bootstrap (OOB or PKI) before they're safe to initiate.

**Stack:** Python, `oqs-python` (liboqs), `pycryptodome`

🔗 [Repo](#) — *(add your repo link)*

---


## 🛡️ Sentinel — Real-Time AI Deepfake Audio Detector

A dual-model ensemble (RawNet2 + AASIST) for detecting AI-generated and manipulated speech in real time — TTS synthesis, voice cloning, GAN vocoders, and replay attacks — with a live call interception pipeline over Twilio Media Streams and sub-3-second detection latency.

**Results:**
| Metric | Cross-Domain (ASVspoof 2019 LA) |
|---|:---:|
| AUC | 0.8845 |
| EER | 19.94% |
| Accuracy | 79.05% |

- Cross-domain evaluation on a benchmark **never seen during training**, proving genuine generalization rather than overfitting to known attack types.
- Dual-model **MAX fusion** strategy — if either model flags a clip, it's flagged — preserving each model's specialist detections (RawNet2 for synthesis artifacts, AASIST for replay/codec attacks).
- Trained on 93,350 clips across 8 sources (ASVspoof5, WaveFake, XTTS v2, Edge-TTS, ReplayDF, LibriSpeech, LJSpeech, VCTK) using multi-GPU DDP on NVIDIA T4s.
- Real-time pipeline: Twilio → FastAPI/WebSocket → 3s rolling window → ensemble inference → kill call if flagged.

**Stack:** PyTorch, FastAPI, WebSockets, Twilio Media Streams, pyroomacoustics

🔗 [Repo](#) — *(add your repo link)*

---

### 🛠️ Tech Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=radical" />
</p>
