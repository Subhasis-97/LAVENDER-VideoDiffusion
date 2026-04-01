# LAVENDER: Latent Adaptive Video Diffusion for Text-Guided Video Editing

LAVENDER is a zero-shot framework for text-guided video editing that produces semantically accurate and temporally consistent results using diffusion models.

## Overview

This project introduces a novel method that performs video editing in latent space using:

- DDIM inversion
- Guided attention blending
- Cross-frame attention

The goal is to enable robust editing without per-video fine-tuning.

## Key Features

- Zero-shot video editing
- Strong semantic alignment with text prompts
- Improved temporal consistency
- Handles large appearance and object changes

## Method

1. Invert video frames into latent space (DDIM inversion)
2. Generate target-aware reference from text prompt
3. Apply guided attention blending during denoising
4. Use cross-frame attention for temporal consistency

## Usage

```bash
git clone https://github.com/Subhasis-97/ABCD.git
cd ABCD
pip install -r requirements.txt

python main.py --input_video input.mp4 --prompt "your prompt"

