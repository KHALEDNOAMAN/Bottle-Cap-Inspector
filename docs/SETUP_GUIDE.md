# Bottle Cap Inspector - Setup Guide

## Prerequisites
- Python 3.8+
- Webcam or video file
- CUDA GPU (optional, for faster inference)

## Installation
```bash
git clone https://github.com/AnkitSaini491/Bottle-Cap-Inspector.git
cd Bottle-Cap-Inspector
pip install -r requirements.txt
```

## Detection Classes
| Class | Description | Color |
|-------|-------------|-------|
| Capped | Bottle with cap on | Green |
| Uncapped | Bottle without cap | Red |

## Running
```bash
# From webcam
python detect.py --source 0

# From video file
python detect.py --source video.mp4

# From image
python detect.py --source image.jpg
```

## Model Performance
| Metric | Value |
|--------|-------|
| mAP@0.5 | ~92% |
| FPS (GPU) | ~30 |
| FPS (CPU) | ~5 |

## Industrial Use Cases
- Quality control on production lines
- Automated bottle sorting
- Packaging verification