<h1 align="center">Cyber-SLA Intelligence for UAV-6G Systems</h1>

<p align="center">
  <a href="https://doi.org/10.71146/kjmr935"><img src="https://img.shields.io/badge/Paper-KJMR-2f6f9f.svg" alt="Paper"></a>
  <a href="uk-conference.ipynb"><img src="https://img.shields.io/badge/Notebook-uk--conference.ipynb-F37626.svg" alt="Notebook"></a>
  <a href="https://www.kaggle.com/nizamuddinmaitlo"><img src="https://img.shields.io/badge/Datasets-Kaggle-20BEFF.svg" alt="Kaggle datasets"></a>
  <a href="https://scholar.google.com/citations?user=bvyKhaEAAAAJ&hl=en"><img src="https://img.shields.io/badge/Publications-Google_Scholar-4285F4.svg" alt="Google Scholar"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/Code_License-MIT-2ea44f.svg" alt="MIT License"></a>
</p>

<p align="center"><b>Nizamuddin Maitlo</b></p>

<p align="center">Joint cyber-risk and SLA prediction for secure UAV-6G aerial cyber-physical systems.</p>

## 🔥 Overview

This project combines malicious-domain detection with next-window SLA prediction for UAV-6G aerial cyber-physical systems. It evaluates cyber risk, communication feasibility, confidence, and joint operational decision rules in a Kaggle-ready workflow.

## ✨ Contributions

- Cyber-risk and SLA prediction in one experimental workflow.
- Leakage-aware splitting and separate model evaluation.
- Confidence-aware joint decision rules.
- Ablation, stress testing, and research-oriented reporting.

## 🧪 Experimental protocol

- The cyber and SLA CSV files are discovered independently under `/kaggle/input`.
- Cyber labels and next-window SLA labels are modeled as separate tasks.
- Joint policy evaluation combines calibrated outputs after task-specific validation.

## 📓 Notebook

The complete experiment is implemented in [uk-conference.ipynb](uk-conference.ipynb). Data discovery, preprocessing, training, evaluation, and export steps are kept together so the workflow can be reviewed and rerun from top to bottom.

## 🛠️ Installation

Create a Python environment and install the listed dependencies:

```bash
python -m pip install -r requirements.txt
```

The notebook is configured for Kaggle. A CUDA-capable GPU is recommended where GPU training is enabled.

## 📦 Datasets

Datasets, trained weights, and generated experiment outputs are not stored in this repository.

| Resource | Purpose | Link |
|---|---|---|
| Malicious Domain Detection Dataset | Cyber-risk prediction | [Kaggle dataset](https://www.kaggle.com/datasets/nizamuddinmaitlo/malicious-domain-detection-dataset) |
| SLA Dataset | Next-window service-level feasibility | [Kaggle dataset](https://www.kaggle.com/datasets/nizamuddinmaitlo/sla-dataset) |

On Kaggle, attach all datasets through **Add Input** before running the notebook. External datasets remain subject to the licenses and terms on their source pages.

## 🚀 Running the experiment

### Kaggle

1. Upload or import [uk-conference.ipynb](uk-conference.ipynb).
2. Attach all datasets listed above through **Add Input**.
3. Enable a GPU accelerator when required by the configured model.
4. Run the notebook from top to bottom.

### Local Jupyter

```bash
python -m pip install -r requirements.txt
jupyter notebook uk-conference.ipynb
```

Dataset paths may need to be changed when running outside Kaggle.

## ♻️ Reproducibility

- Keep the documented train, validation, and test protocol unchanged when comparing models.
- Fit thresholds, calibration parameters, and feature transformations without using final test labels.
- Record the random seed, package versions, accelerator, and dataset version for each run.
- Treat saved tables and figures under the notebook's output directory as generated artifacts rather than source files.

## 📚 Paper information

The publications below provide the closest published context for the malicious-domain decision pipeline and confidence/SLA-gated UAV perception.

| Publication | Venue | Year | Link |
|---|---|---:|---|
| AGENT-MD: A Human-Governed Agentic AI Framework for Explainable and Uncertainty-Aware Malicious Domain Detection | Kashf Journal of Multidisciplinary Research, 3(3), 478–491 | 2026 | [DOI](https://doi.org/10.71146/kjmr935) |
| Risk-Aware Edge-Assisted UAV Perception with Confidence and SLA Gating | Machines, 14(6), 685 | 2026 | [DOI](https://doi.org/10.3390/machines14060685) |

## ⭐ Citation

For research building on this repository, cite the relevant publication or dataset descriptor:

```bibtex
@article{shaikh2026agentmd,
  title   = {AGENT-MD: A Human-Governed Agentic AI Framework for Explainable and Uncertainty-Aware Malicious Domain Detection},
  author  = {Shaikh, Bushra and Mal, Khakoo and Shaikh, Noor Ahmed and Maitlo, Nizamuddin},
  journal = {Kashf Journal of Multidisciplinary Research},
  volume  = {3},
  number  = {3},
  pages   = {478--491},
  year    = {2026},
  doi     = {10.71146/kjmr935}
}
```

```bibtex
@article{maitlo2026riskaware,
  title   = {Risk-Aware Edge-Assisted UAV Perception with Confidence and SLA Gating},
  author  = {Maitlo, Nizamuddin and Arain, Rafaqat Hussain and Arshid, Kaleem and Noonari, Nooruddin and Mustafa, Ghulam},
  journal = {Machines},
  volume  = {14},
  number  = {6},
  pages   = {685},
  year    = {2026},
  doi     = {10.3390/machines14060685}
}
```

## ⚠️ Scope and limitations

The cyber and SLA datasets are independent rather than synchronized observations from the same UAV missions. Joint results should be interpreted as a modular stress test, not an end-to-end physical-flight validation.

## 📄 License

Repository code is released under the [MIT License](LICENSE). Datasets and publications retain their own licenses and terms.

## 🤝 Acknowledgements

The experiments use public datasets, open-source Python libraries, and Kaggle compute infrastructure. We thank the dataset contributors and software maintainers who support reproducible research.
