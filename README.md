## Reproducibility Information for "Simulating Textual Transmission with Natural Language Processing Techniques"

This repository contains the code and data for the paper "*Simulating Textual Transmission with Natural Language Processing Techniques*".

### 🔧 Software Dependencies

The code was developed and tested in a **Google Colab** environment with the following package versions:

```python
# Core Python
Python 3.10.12
numpy==1.25.0
pandas==2.2.2
scipy==1.15.3

# NLP & Machine Learning
transformers==4.52.2
sentence-transformers==4.1.0
datasets==2.14.4
torch==2.6.0+cu124
openai==1.81.0

# Phylogenetics & Visualization
ete3==3.1.3
networkx==3.4.2
matplotlib==3.10.0
seaborn==0.13.2
biotite==0.3.0
python-levenshtein==0.21.1

# Google Colab
google-colab==1.0.0
```

### 💻 Hardware Requirements

- **Environment**: Google Colab
- **GPU**: Tesla T4 (15GB RAM)
- **RAM**: 12.7 GB
- **Storage**: ~2GB free space for models and datasets

### ⏱️ Runtime Information

- **Total execution time**: ~1 hour
- **Breakdown**:
  - Data generation and preprocessing: ~15 minutes
  - Tree reconstruction experiments: ~20 minutes  
  - Text reconstruction experiments: ~15 minutes
  - LLM-based simulations: ~10 minutes

### 🎲 Random Seed

All stochastic processes can use the fixed random seed:
```python
random_seed = 42
np.random.seed(42)
random.seed(42)
torch.manual_seed(42)
```

### 🚀 Quick Start

1. Upload the notebook to Google Colab
2. Ensure GPU runtime is enabled (Runtime → Change runtime type → GPU)
3. Run all cells sequentially
4. Results will be saved automatically in the Colab environment

### 📁 Repository Structure

```
YOUR_PATH
  |---Notebook : Simulating Text Transmission.ipynb
  |---confusion_matrix.npy
  |---files
      |---echoes.json
```

### 📝 Notes

- The code is optimized for Colab environment
- Some LLM operations require API keys (handled via Colab secrets)
- Results may vary slightly due to GPU floating-point precision, but overall conclusions remain stable

