# ML-Project: Voice Conversion with Diffusion Models

A real-time voice conversion system using diffusion-based generative modeling to transform a source speaker’s voice into a target speaker’s, with minimal latency and high audio fidelity.

## 🚀 Features

- **Diffusion-based conversion**: Leverages recent advances in denoising diffusion probabilistic models for high-quality voice style transfer.  
- **Real-time inference**: Optimized pipelines and optional model distillation for near-live conversion performance.  
- **Multi-stage training**:  
  1. Train from scratch (`train.sh` / `train_v1.sh`)  
  2. Fine-tune on pre-trained Russian checkpoints (`load_rus_checkpoints.py`)  
  3. Distillation pipeline for fast-run models (`run_distill.sh`)  
- **Easy demos & evaluation**:  
  - `run_demo_v2.sh`, `run_demo_compare.sh` for side-by-side audio comparison  
  - `eval.sh` generates spectrograms and metrics in `eval_plots/`

## 📁 Repository Structure
├── dataset/ # Preprocessed audio data

├── seed-vc*/ # Minimal baseline implementations

├── eval_plots/ # Generated evaluation figures

├── load_rus_checkpoints.py # Download or prepare Russian model weights

├── train.sh, train_v1.sh # Training scripts

├── run_inference.sh # Inference script

├── run_demo_*.sh # Demo & comparison scripts

├── run_distill.sh # Distillation pipeline

├── eval.sh # Evaluation workflow

├── test.ipynb # Quick notebook tests

├── requirements.txt # Python dependencies

└── README.md # ← this file


## ⚙️ Installation

Clone the repo:  
   ```bash
   git clone https://github.com/VladimirZelenokor1/ML-Project---Voice-Conversion-with-Diffusion-Models.git
   cd ML-Project---Voice-Conversion-with-Diffusion-Models

"""
python3 -m venv venv && source venv/bin/activate
"""

"""
pip install --upgrade pip
pip install -r requirements.txt
"""

##  📊 Results
Converted audio samples and spectrogram comparisons are saved under eval_plots/. Check the demo scripts for side-by-side WAV outputs.



