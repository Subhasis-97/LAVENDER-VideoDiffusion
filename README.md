# LAVENDER-VideoDiffusion

Official implementation of **LAVENDER: Latent Adaptive Video Diffusion for Text-Guided Video Editing with Attention Blending**.

## Overview

LAVENDER is a zero-shot framework for text-guided video editing that generates semantically accurate and temporally consistent videos using diffusion models.

The method operates in latent space and introduces guided attention blending to improve editing quality, especially for challenging transformations.

## Key Features

- Zero-shot video editing (no per-video training required)
- Strong semantic alignment with text prompts
- Temporal consistency across frames
- Robust to large appearance and object changes

## Method

1. **DDIM Inversion** – Convert input video into latent space  
2. **Reference Generation** – Create target-aware visual guidance from prompt  
3. **Guided Attention Blending** – Inject target semantics during denoising  
4. **Cross-Frame Attention** – Maintain temporal coherence  

## Installation

```bash
git clone https://github.com/Subhasis-97/LAVENDER-VideoDiffusion.git
cd LAVENDER-VideoDiffusion

pip install -r requirements.txt
