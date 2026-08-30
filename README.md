# Cyber-SLA Intelligence for UAV-6G Systems

Joint cyber-risk and SLA prediction for secure UAV-6G aerial cyber-physical systems.

## Overview

This project combines malicious-domain detection with service-level prediction for UAV-6G aerial cyber-physical systems. It evaluates cyber risk, next-window SLA reliability, confidence, and joint operational decision rules in a GPU-ready Kaggle workflow.

## Highlights

- Cyber-risk and SLA prediction
- Leakage-aware data splitting
- Confidence-aware joint decisions
- Ablation, stress-test, and paper-ready reporting

## Notebook

The full experiment is provided in [uk-conference.ipynb](uk-conference.ipynb). It is configured for Kaggle and expects the datasets described in the notebook to be attached through the **Add Input** panel.

## Running the experiment

1. Create a Kaggle notebook or open the included notebook in Jupyter.
2. Attach the required dataset and enable a GPU accelerator where noted.
3. Install the listed dependencies.
4. Run the notebook from top to bottom.

```bash
pip install -r requirements.txt
```

Datasets, trained weights, and generated experiment outputs are not stored in this repository.

## License

This project is available under the MIT License.
