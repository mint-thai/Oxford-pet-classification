# Oxford Pet Breed Classification

Classifying 37 cat and dog breeds using PyTorch and transfer learning (ResNet-50) on the Oxford-IIIT Pet Dataset.

## Setup

### Option 1: CPU (default)

Works on any machine. No API keys required.

```bash
git clone https://github.com/mint-thai/Oxford-pet-classification.git
cd Oxford-pet-classification

python -m venv venv

# macOS/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate

pip install -r requirements.txt
```

### Option 2: GPU (CUDA)

For NVIDIA GPUs. Follow the same steps as above, then replace the PyTorch install:

```bash
git clone https://github.com/mint-thai/Oxford-pet-classification.git
cd Oxford-pet-classification

python -m venv venv

# macOS/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate

pip install -r requirements.txt
pip uninstall torch torchvision
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
```

> **Apple Silicon:** MPS is auto-detected. No extra steps needed — just use the CPU path above.

## Run

```bash
jupyter notebook Oxford_Pet_Classification.ipynb
```

Run all cells top-to-bottom. The dataset (~800 MB) downloads automatically on first run.
