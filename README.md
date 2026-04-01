# 🌿 LAVENDER-VideoDiffusion

🚀 Official implementation of  
**LAVENDER: Latent Adaptive Video Diffusion for Text-Guided Video Editing with Attention Blending**

---

## 📌 Overview

LAVENDER is a **zero-shot video editing framework** that enables high-quality, text-guided video manipulation using diffusion models—without requiring per-video fine-tuning.

The framework operates in the **latent space** and introduces a novel **Guided Attention Blending** mechanism to achieve:

- Strong semantic alignment with text prompts  
- High temporal consistency across frames  
- Robust editing under large appearance and structural changes  

---

## ✨ Highlights

- 🔹 Zero-shot video editing (no retraining required)  
- 🔹 Works with pretrained diffusion models  
- 🔹 Maintains motion and structure consistency  
- 🔹 Handles complex edits (object replacement, appearance change)  
- 🔹 Efficient and modular pipeline  

---

## 🧠 Method Overview

LAVENDER consists of four key steps:

1. **DDIM Inversion**  
   Convert input video frames into latent representations.

2. **Reference Generation**  
   Generate a target-aware visual reference from the text prompt.

3. **Guided Attention Blending**  
   Blend source and target attention maps during denoising for precise editing.

4. **Cross-Frame Attention**  
   Propagate temporal information across frames to ensure smooth and consistent results.

---

## ⚙️ Installation

```bash
git clone https://github.com/Subhasis-97/LAVENDER-VideoDiffusion.git
cd LAVENDER-VideoDiffusion

pip install -r requirements.txt
