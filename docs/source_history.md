# Source history

This project combines a cleaned local portfolio snapshot with the existing owned repository, https://github.com/Qimatxbase/MultiCameraTracking. The existing repository and its history are retained during consolidation.

Original source repositories:

- https://github.com/Quang0309/MultiCameraTracking

Original local Git databases, branch states and recovery copies are retained outside the public repositories in the workspace .maintenance/ directory.

## Preserved implementation variants

The existing owned repository contributes the distinct `download.ipynb`, `train_osnet_kaggle.ipynb`, `fix_configs3.py` and `scripts/train_osnet.py` workflows. Restored notebooks retain their cell source with outputs and execution metadata removed.

`configs/mevid_osnet_baseline.yml` preserves the original plain OSNet configuration from the owned repository. The restored `scripts/train_osnet.py` runner points to this baseline. `configs/mevid_osnet.yml` retains the separate local OSNetMGN configuration, with its missing `DATASETS` mapping header restored. The local Kaggle workflow remains in `Kaggle_run/`; it is a distinct experiment rather than a duplicate notebook.
