# COMP 3610: Big Data Analytics - Assignment 2

ML Model Training & Evaluation using the NYC Yellow Taxi Trip dataset.

---

## Requirements

- Python 3.10+
- CUDA-compatible GPU (optional, CPU supported)

---

## Setup

**1. Clone the repository**

```
git clone https://github.com/JOSIAHTHEPROGRAMMER/ML-Model-Training---Evaluation
cd ML-Model-Training---Evaluation
```

**2. Install dependencies**

```
pip install -r requirements.txt
```

For GPU support, install PyTorch with CUDA before running the above:

```
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
```

**3. Launch Jupyter**

```
jupyter notebook
```

**4. Open and run `assignment2.ipynb`**

The notebook will automatically download the required dataset files on first run. No manual data setup is needed.

---

## Project Structure

```
assignment2.ipynb       main notebook
requirements.txt        python dependencies
README.md               this file
.gitignore              excludes data and model files
data/                   auto-created on first run (gitignored)
```

---

## Notes

- Data files are downloaded programmatically and excluded from version control.
- All random operations use `random_state=42` for reproducibility.
- Hyperparameter tuning uses a stratified sample of 200,000 rows to keep runtimes manageable.
- Final model evaluation uses the full dataset.
