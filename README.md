<div align="center">

  <!-- Your header GIF -->

  <img src="assets/gif_77e877d66047.gif">



  <br>

  <br>



  <img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=700&size=27&duration=4000&pause=1000&color=FF007F&center=true&vCenter=true&width=1000&lines=Hey+%3A%29;I%27m+an+Undergrad+in+Computer+Science+and+Applied+Mathematics;Check+out+my+work+%28%EF%BF%A3%E2%96%BD%EF%BF%A3%29" alt="Typing SVG" />

</div>



<br>

<br>

<div align="left"><img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=700&size=24&color=FF007F&repeat=false&width=450&lines=%5B+%2F%2F+FEATURED_PROJECTS_+%5D" alt="Featured Projects" align="absmiddle" />&nbsp;<img src="https://play.pokemonshowdown.com/sprites/gen5ani/gengar.gif" width="57" align="text-top" /></div>

<br>

---

### [QRYPTEX](https://github.com/nishulucyna/techfest)
**Hybrid Post-Quantum Cryptographic (PQC) Protocol**

A robust encryption pipeline combining traditional symmetric cryptography with NIST-standardized quantum-resistant algorithms to thwart "Harvest Now, Decrypt Later" attacks.

#### Core Constructs
* **KEM:** ML-KEM (CRYSTALS-Kyber) for quantum-resistant shared secrets.
* **DSA:** ML-DSA (CRYSTALS-Dilithium) for origin authentication.
* **ENC:** AES-256-GCM bulk encryption via Kyber shared secrets.

#### Architecture & Findings
Simulated end-to-end flow. Identified a critical limit in QRNG-based commitments lacking origin authentication. Out-of-Band (OOB) channels remain mandatory for initial key exchange against MITM attacks.

---

### [SENTINEL](https://github.com/CRRAO-Internal-Hackathon-2026/techfest)
**Real-Time AI Deepfake Audio Detector**

A dual-model ensemble system designed to detect AI-generated and manipulated speech in real-time, featuring a live call interception pipeline with sub-3-second latency.

#### Core Architecture
* **Ensemble Strategy:** MAX fusion of RawNet2 (synthesis artifact detection) and AASIST (spectral-temporal graph analysis) to catch both advanced TTS cloning and replay attacks.
* **Live Pipeline:** Twilio Media Streams → WebSocket → 3-second rolling analysis window → automated call termination upon deepfake detection.
* **Tech Stack:** PyTorch, FastAPI, WebSockets, Twilio, Gradio.

#### Training & Performance
* **Dataset:** Trained on 93,000+ clips across modern attack vectors (ASVspoof5, XTTS v2, WaveFake, Edge-TTS).
* **Results:** Achieved and demonstrated genuine zero-shot generalization with **0.8845 AUC** on unseen cross-domain benchmarks (ASVspoof 2019 LA).

---

<br>
### `[ // ONGOING PROJECTS_ ]`
#### Nothing atm! (；￣Д￣)
---
<div align="center">
  <sub><i>// Connection Terminated - Last Updated: June 2026</i></sub>
</div>
