# Flower-Recognition-System
Computer Vision with Pytorch


# Flower Recognition System - GreenTech Solutions Ltd.

Computer Vision project for binary flower image classification (`Daisy` vs `Dandelion`) using transfer learning in PyTorch.

## Project Context

GreenTech Solutions Ltd. needs an automated vision system to classify flowers in real-time agricultural settings.  
This project implements the end-to-end ML workflow in a single notebook:

- Environment setup and dependencies
- Dataset download and extraction
- Exploratory Data Analysis (EDA)
- Data preprocessing and augmentation
- Model building with transfer learning (`timm`)
- Training and validation
- Test evaluation (F1-score as primary metric)
- Inference, error analysis, and Grad-CAM explainability
- Results discussion and future improvements

## Repository Contents

- `GreenTech_Flower_Recognition.ipynb` - complete notebook pipeline
- `requirements.txt` - Python dependencies

## Tech Stack

- Python
- PyTorch (`torch`, `torchvision`)
- `timm` (pretrained model backbones)
- `pytorch-grad-cam` (visual explanations)
- `torchmetrics`
- `numpy`, `pandas`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `Pillow`

## Setup

### 1) Create and activate a virtual environment

Windows (PowerShell):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

macOS/Linux (bash):

```bash
python -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies

```bash
pip install -r requirements.txt
```

## How to Run

1. Start Jupyter:
   ```bash
   jupyter notebook
   ```
2. Open `GreenTech_Flower_Recognition.ipynb`.
3. Run all cells in order (`Kernel > Restart & Run All`) to reproduce the pipeline.

## Notebook Workflow

The notebook is organized as:

1. Project overview and goals
2. Environment setup
3. Dataset acquisition and extraction
4. EDA and class inspection
5. Preprocessing and data augmentation
6. Transfer learning model definition (`timm`)
7. Training loop
8. Test set evaluation
9. Inference and error analysis
10. Grad-CAM visualization and discussion

## Evaluation

- **Task:** Binary classification (`Daisy` vs `Dandelion`)
- **Primary metric:** F1-score


## Explainability

Grad-CAM is used to visualize which image regions influence predictions, helping with:

- Model debugging
- Error interpretation
- Trust and transparency for deployment decisions

## Future Improvements

- Hyperparameter tuning (learning rate, scheduler, batch size)
- Compare multiple pretrained backbones
- Add cross-validation and stronger robustness checks
- Improve data quality and class balance handling
- Package inference as an API or lightweight app

## Author

AI Engineer Cristian L.

## License

MIT
