# SmishDetect-LLM

> A multilingual SMS phishing (smishing) detection framework leveraging Large Language Models across Bengali, English, Banglish, and Code-Mixed linguistic varieties.

---

## Overview

**SmishDetect-LLM** is a research framework for detecting smishing (SMS-based phishing) attacks in multilingual contexts. The framework evaluates both BERT-based encoder models and GPT-based decoder models across two experimental versions:

- **Baseline Version** — Models trained on Bengali and English data only.
- **Proposed Version** — Models trained on all four linguistic varieties: Bengali, English, Banglish, and Code-Mixed.

This repository contains the complete source code, data preprocessing scripts, model training pipelines, and evaluation utilities used in the associated thesis.

---

## Repository Structure

```
SmishDetect-LLM/
├── BERT_Based_Base_Version.ipynb       # BERT Baseline experiments
├── BERT_Based_Proposed_Version.ipynb   # BERT Proposed experiments
├── GPT_Based_Base_Version.ipynb        # GPT Baseline experiments
├── GPT_Based_Proposed_Version.ipynb    # GPT Proposed experiments
└── README.md
```

---

## Experiments

Four Google Colab notebooks implement the complete experiments. Each can be run directly in Google Colab with GPU acceleration.

### BERT-Based Models

| Notebook | Description | Link |
|----------|-------------|------|
| Baseline Version | All BERT-based encoder models trained on Bengali & English data only | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/shariul-islam-au/SmishDetect-LLM/blob/main/BERT_Based_Base_Version.ipynb) |
| Proposed Version | All BERT-based encoder models trained on all four linguistic varieties | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/shariul-islam-au/SmishDetect-LLM/blob/main/BERT_Based_Proposed_Version.ipynb) |

### GPT-Based Models

| Notebook | Description | Link |
|----------|-------------|------|
| Baseline Version | GPT-based decoder models trained on Bengali & English data only | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/shariul-islam-au/SmishDetect-LLM/blob/main/GPT_Based_Base_Version.ipynb) |
| Proposed Version | GPT-based decoder models trained on all four linguistic varieties | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/shariul-islam-au/SmishDetect-LLM/blob/main/GPT_Based_Proposed_Version.ipynb) |

---

## Linguistic Varieties Covered

| Variety | Description |
|---------|-------------|
| **Bengali** | Native Bengali script SMS messages |
| **English** | Standard English SMS messages |
| **Banglish** | Bengali language written in Roman/Latin script |
| **Code-Mixed** | Messages mixing Bengali and English within the same text |

---

## Getting Started

### Prerequisites

- Python 3.8+
- A Google account (for running Colab notebooks)
- GPU runtime recommended (available free via Google Colab)

### Running the Notebooks

1. Click any of the **Open in Colab** badges above, or navigate to the notebook in this repository.
2. In Colab, go to **Runtime → Change runtime type** and select **GPU**.
3. Run all cells in order. Each notebook is self-contained and will install its own dependencies.

### Running Locally

```bash
# Clone the repository
git clone https://github.com/shariul-islam-au/SmishDetect-LLM.git
cd SmishDetect-LLM

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

## Models

The framework evaluates the following model families:

**Encoder Models (BERT-based)**
- mBERT (Multilingual BERT)
- BanglaBERT
- Other task-specific BERT variants

**Decoder Models (GPT-based)**
- Multilingual GPT-based causal language models fine-tuned for classification

---

## Evaluation

Each notebook includes a complete evaluation pipeline reporting:

- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- Per-class performance across linguistic varieties

---

## Citation

If you use this work in your research, please cite:

```bibtex
@thesis{islam2025smishdetect,
  title     = {SmishDetect-LLM: Multilingual SMS Phishing Detection Using Large Language Models},
  author    = {Shariul Islam},
  year      = {2025},
  school    = {Murdoch University},
  note      = {Available at: https://github.com/shariul-islam-au/SmishDetect-LLM}
}
```

---

## License

This project is released for academic and research purposes. See [LICENSE](LICENSE) for details.

---

## Contact

**Shariul Islam**  
Email: [shariul.islam.au@gmail.com](mailto:shariul.islam.au@gmail.com)
