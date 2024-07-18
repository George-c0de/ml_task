# CLIP ChartLlama Dataset Training

This repository contains code to fine-tune OpenAI's CLIP model on the ChartLlama dataset. The dataset includes pairs of images and conversations that describe the images. The goal is to train the CLIP model to better understand and represent these pairs.

## Requirements
- PyTorch
- Transformers library from Hugging Face
- Datasets library from Hugging Face
- PIL (Pillow)
- requests
- pandas

## Setup

1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```

2. Install the required Python packages:
    ```bash
    pip install jupyter
    ```

## Usage

### Determine Device

By default, the code uses the CPU for training. Modify the `device` variable to use a GPU if available:
```python
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
