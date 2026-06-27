# NVIDIA Nemotron Reasoning Challenge Archive

This archive preserves the historical competition work that fed into the early Nemotron experimentation around Manatuabon.

It is not the live Manatuabon application.

The purpose of this archive is to keep:
- the Kaggle and Colab training flow
- the synthetic reasoning dataset generation scripts
- the demo and inference notebooks
- the submission history and external artifacts trail

The live observatory runtime remains in Manatuabon and should stay there.

## What This Archive Contains

- `kaggle_pipeline.py`: builds the synthetic reasoning training traces
- `kaggle_ensemble_mix.py`: merges legacy and CoVe-style traces into the final ensemble dataset
- `nemotron_self_play_vllm.py`: local self-play and LoRA inference experiment
- `nvidia-nemotron-submission-demo.ipynb`: competition demo notebook snapshot
- `train_lora_colab.ipynb`: Colab LoRA training notebook
- `train_manatuabon_qlora_colab.ipynb`: later QLoRA notebook connected to the broader project direction
- `synthetic_cot.jsonl`, `synthetic_cot_grandmaster.jsonl`, `master_ensemble_dataset.jsonl`: training corpora
- `train.csv`, `test.csv`: challenge data snapshot currently available locally
- `downloads/`: extra notebooks and scratch files found in Downloads
- `drive_colab/`: mounted Google Drive Colab notebook variants imported from `G:\My Drive\Colab Notebooks`
- `drive_lora/`: lightweight metadata imported from `G:\My Drive\nemotron_reasoning_lora`

## What Stays In Manatuabon

The following are active application surfaces, not archive material:
- the packaged Nemotron runtime client in `manatuabon/core/nemotron_client.py`
- query/chat bridge integration in `manatuabon/bridge/manatuabon_bridge.py`
- ingest and consolidation agents under `manatuabon/core/`
- council/governance logic under `manatuabon/governance/`
- active tests and operational docs tied to the observatory runtime

Those files depend on Nemotron as a live model backend for the observatory. They should not be moved into this archive repo.

## External Assets Not Vendored Here

Large or environment-specific files were intentionally left out of this archive staging folder:
- `submission.zip` through `submission15.zip` in Downloads
- LoRA adapter weights inside those submission ZIPs
- LoRA adapter weights and checkpoint directories from `G:\My Drive\nemotron_reasoning_lora`
- any additional Google Drive notebook copies outside the imported Nemotron set
- Colab runtime outputs saved outside this workspace
- `kaggle.json` credentials files

See `EXTERNAL_IMPORT_CHECKLIST.md` for the follow-up import list and `DRIVE_LORA_MANIFEST.md` for the mounted adapter inventory.

## Why This Archive Exists

This challenge work is historically useful because it shows:
- how the synthetic reasoning datasets were generated
- how LoRA and QLoRA experiments were organized
- what was shipped as competition submissions
- which artifacts later influenced Manatuabon's local-model direction

It should be read as a lessons-learned engineering archive, not as the canonical source for the live observatory.