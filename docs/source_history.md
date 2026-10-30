# Source history

This project combines a cleaned local portfolio snapshot with the existing owned repository, https://github.com/Qimatxbase/MultiCameraTracking. The existing repository and its history are retained during consolidation.

Original source repositories:

- https://github.com/Quang0309/MultiCameraTracking

Original local Git databases, branch states and recovery copies are retained outside the public repositories in the workspace .maintenance/ directory.

## Preserved implementation variants

The existing owned repository contributes the distinct `notebooks/download_mevid.ipynb`, `notebooks/osnet_kaggle.ipynb`, `scripts/normalize_solver_config.py` and `scripts/train_osnet.py` workflows. Restored notebooks retain their cell source with outputs and execution metadata removed.

`configs/mevid_osnet_baseline.yml` preserves the original plain OSNet configuration from the owned repository. The restored `scripts/train_osnet.py` runner points to this baseline. `configs/mevid_osnet.yml` retains the separate local OSNetMGN configuration, with its missing `DATASETS` mapping header restored. The local Kaggle workflow remains in `notebooks/osnet_mgn_kaggle.ipynb`; it is a distinct experiment rather than a duplicate notebook.

## Descriptive filenames — 31 October 2026

Source content and distinct experiments were retained while filenames were clarified. Original filenames remain recorded below for provenance.

| Original path | Current path |
| --- | --- |
| `Kaggle_run/train-osnet-kaggle.ipynb` | `notebooks/osnet_mgn_kaggle.ipynb` |
| `train_osnet_kaggle.ipynb` | `notebooks/osnet_kaggle.ipynb` |
| `download.ipynb` | `notebooks/download_mevid.ipynb` |
| `scripts/agw_resnet_ibn_25740743.ipynb` | `notebooks/agw_resnet50_ibn_kaggle.ipynb` |
| `fix_configs3.py` | `scripts/normalize_solver_config.py` |
