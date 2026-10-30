# Multi-Camera Person Re-Identification

MEVID person re-identification experiments comparing CNN architectures under camera and clothing changes.

**Technologies:** Python · PyTorch · FastReID · Streamlit

## Academic context and contribution

Created for **UTS 42177, Team 8** as a comparative person re-identification research project.

The documented contribution split is:

- **Khanh Hoang Nguyen:** OSNet data preparation, training, Rank-1 and mAP evaluation, and integration.
- **Quang:** the shared framework, data loaders and AGW-ResNet50-IBN work.
- **Hung:** BoT-ResNet50 work.

The repository preserves both the plain OSNet workflow and a distinct OSNet-MGN experiment. Broader comparison and application components retain their team and upstream attribution.

## What is included

- BoT-ResNet50, AGW-ResNet50-IBN and OSNet/MGN research configurations.
- General, same-outfit and cross-outfit evaluation protocols.
- Gallery indexing, similarity search, detection and tracking modules.

## Setup

```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Run

```bash
streamlit run app/app.py
```

The MEVID dataset, pretrained weights and training dependencies must be supplied separately. See docs/original_readme.md for training and evaluation details. This is team research; the inherited documentation records the wider comparison.

## Source and credits

This portfolio snapshot preserves work from the following repositories. Existing author credits, citations and license files are retained; team and upstream code are not presented as solely authored work.

- https://github.com/Quang0309/MultiCameraTracking

[Portfolio index](https://github.com/Qimatxbase/engineering_portfolio)
