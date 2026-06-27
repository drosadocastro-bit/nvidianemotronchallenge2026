# Notebook Review

This review focuses on the notebooks imported into `drive_colab/` and identifies which ones look strongest for public preservation versus which ones appear to be duplicates, partial copies, or weak historical variants.

## Strong Keep Candidates

- `drive_colab/train_lora_colab.ipynb`
  - 9 cells
  - likely the most polished direct LoRA training notebook in the set
- `drive_colab/train_lora_colab (1).ipynb`
  - 8 cells
  - large file and likely a richer earlier variant worth preserving
- `drive_colab/train_lora_colab (2).ipynb`
  - 7 cells
  - another substantial variant that may capture a meaningful iteration
- `drive_colab/train_lora_colab (4).ipynb`
  - 7 cells
  - moderate-size variant, likely still useful historically
- `drive_colab/unsloth_colab_microtune.ipynb`
  - 3 cells
  - large enough to suggest substantive content despite low cell count
- `drive_colab/nemotron_self_play_vllm.ipynb`
  - 2 cells
  - distinct experiment branch, not just another training copy

## Likely Weak Or Duplicate Variants

- `drive_colab/train_lora_colab (3).ipynb`
  - 7 cells but only about 7 KB
  - likely a stripped or broken copy rather than a full notebook
- `drive_colab/train_lora_colab (5).ipynb`
  - 7 cells but only about 6 KB
  - likely another incomplete or near-empty variant
- `drive_colab/Copy of unsloth_colab_microtune.ipynb`
  - 1 cell and much smaller than the main `unsloth_colab_microtune.ipynb`
  - likely a scratch duplicate rather than the canonical notebook

## Recommended Public Strategy

The public archive has now been trimmed accordingly:

1. `train_lora_colab (3).ipynb` was removed
2. `train_lora_colab (5).ipynb` was removed
3. `Copy of unsloth_colab_microtune.ipynb` was removed

The stronger notebook variants remain in place.

## Prior Review Logic

If the goal is a cleaner public-facing archive while still preserving history:

1. keep all notebooks in git for now because they are part of the historical record
2. treat the weak variants as low-priority duplicates in the docs
3. if you later want a tighter archive, remove `train_lora_colab (3).ipynb`, `train_lora_colab (5).ipynb`, and `Copy of unsloth_colab_microtune.ipynb` first

## Why I Did Not Delete Them Automatically

The current evidence is structural, not semantic. File size and cell count strongly suggest weaker copies, but that is not enough reason to erase history without your explicit approval.