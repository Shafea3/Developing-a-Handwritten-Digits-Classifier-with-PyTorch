# MNIST Handwritten Digits Classifier

A simple, well-documented PyTorch notebook for classifying MNIST handwritten digits. This repo aims to be reproducible and easy to run locally or in the cloud.

This project is adapted from the AWS Machine Learning Fundamentals Nanodegree Program's second course (Introduction to Deep Leraning) on Udacity. It follows the course’s learning objectives and structure with a few additions for reproducibility and documentation.

## What’s inside

- Jupyter Notebook: `MNIST_Handwritten_Digits-STARTER.ipynb`
- Minimal training pipeline for MNIST (PyTorch + TorchVision)
- Optional model artifact: `mnist_model.pth`
- Data directory (ignored by default): `data/`

## Quickstart

### 1) Create and activate an environment (optional but recommended)

```bash
# macOS/Linux
python -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies

```bash
pip install -r requirements.txt
```

Tip: If you have a compatible GPU, install the appropriate PyTorch build from https://pytorch.org/get-started/locally/.

### 3) Launch Jupyter

```bash
python -m ipykernel install --user --name mnist-kernel
jupyter notebook
```

Open `MNIST_Handwritten_Digits-STARTER.ipynb` and run cells top-to-bottom.

## Data

The notebook can download MNIST automatically via `torchvision.datasets.MNIST` into `./data/` if it isn’t present. The `data/` folder is ignored by Git to keep the repo small.

## Tips

- Reproducibility: We set deterministic seeds in the first setup cell. Small variations can still occur across platforms/backends.
- Artifacts: If you save trained models, prefer Git LFS or attach them to a GitHub Release. By default, `*.pth` files are git-ignored.

## Repository structure

MNIST Classifier/

- MNIST_Handwritten_Digits-STARTER.ipynb
- README.md
- requirements.txt
- data/ (created/filled at runtime; ignored)
- mnist_model.pth (optional saved weights; ignored by git)
- .gitignore

## License

Code in this repository is released under the MIT License (see `LICENSE`).

Notes:

- The MNIST dataset is distributed via TorchVision and is governed by its respective license/terms.
- Educational attribution: Adapted from the AWS ML Fundamentals Nanodegree's 2nd course (Introduction to Deep Learning) on Udacity. Any course materials remain the property of their respective owners.

## Acknowledgments

- AWS Machine Learning Fundamentals Nanodegree on Udacity
- PyTorch and TorchVision teams
