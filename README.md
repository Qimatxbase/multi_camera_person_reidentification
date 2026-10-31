# Multi-Camera Person Re-Identification

MEVID person re-identification experiments comparing CNN architectures under camera and clothing changes.

**Technologies:** Python · PyTorch · FastReID · Streamlit

## Academic context and contribution

Created for **UTS 42177, Team 8** as a comparative person re-identification research project.

The documented contribution split is:

- **Khanh Hoang Nguyen:** OSNet data preparation, training, and Rank-1 and mAP evaluation. The team documentation also credits embedding-integration work; the reusable application in this checkout remains partially integrated.
- **Quang:** the shared framework, data loaders and AGW-ResNet50-IBN work.
- **Hung:** BoT-ResNet50 work.

The repository preserves both the plain OSNet workflow and a distinct OSNet-MGN experiment. Broader comparison and application components retain their team and upstream attribution.

## What is included

- BoT-ResNet50, AGW-ResNet50-IBN and OSNet/MGN research configurations.
- General, same-outfit and cross-outfit evaluation protocols.
- Gallery indexing, similarity search, detection and tracking scaffolding.

The implemented OSNet research path is retained in `notebooks/osnet_kaggle.ipynb`, `notebooks/osnet_mgn_kaggle.ipynb`, `scripts/train_osnet.py` and `scripts/eval_mevid_protocols.py`.

## Setup

```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Run

The following command launches the retained Streamlit UI scaffold:

```bash
streamlit run app/app.py
```

The application needs integration fixes before use: its entrypoint calls page `render()` functions while the page modules expose `main()`, and the reusable feature extractor's OSNet and TransReID branches raise `NotImplementedError`. These gaps are separate from the OSNet research training and evaluation workflows above.

The MEVID dataset, pretrained weights and training dependencies must be supplied separately. See docs/original_readme.md for training and evaluation details. This is team research; the inherited documentation records the wider comparison.

## Source and credits

This portfolio snapshot preserves work from the following repositories. Existing author credits, citations and license files are retained; team and upstream code are not presented as solely authored work.

- https://github.com/Quang0309/MultiCameraTracking

[Portfolio index](https://github.com/Qimatxbase/engineering_portfolio)
