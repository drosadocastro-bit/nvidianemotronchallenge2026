# NVIDIA Nemotron Reasoning Challenge Archive

Historical archive of my NVIDIA Nemotron 2026 reasoning challenge workflow, preserving synthetic reasoning data generation, Colab fine-tuning notebooks, LoRA packaging, inference experiments, and lessons learned.

This is not the live Manatuabon application.

## At A Glance

- Preserves the competition training and inference workflow
- Keeps the synthetic reasoning dataset generation scripts
- Captures Colab, Kaggle, and local Nemotron experiment paths
- Records the submission trail without committing heavyweight binaries
- Separates historical challenge artifacts from the live Manatuabon runtime

## Start Here

- `LESSONS_LEARNED.md`: what worked, what changed, and what this archive preserves
- `TIMELINE.md`: chronological view of the competition workflow and later consolidation
- `PROJECT_STATUS.md`: current archive scope and what remains external

## What This Archive Contains

- `kaggle_pipeline.py` and `kaggle_ensemble_mix.py`: synthetic reasoning dataset generation
- `nemotron_self_play_vllm.py`: local experiment path
- `nvidia-nemotron-submission-demo.ipynb`: competition demo notebook snapshot
- `train_lora_colab.ipynb` and `train_manatuabon_qlora_colab.ipynb`: training notebook path
- `synthetic_cot.jsonl`, `synthetic_cot_grandmaster.jsonl`, `master_ensemble_dataset.jsonl`: preserved training corpora
- `downloads/`: extra local notebook and scratch artifacts from Downloads
- `drive_colab/`: imported Google Drive Colab notebook variants
- `drive_lora/`: lightweight metadata from the mounted LoRA export

For the detailed inventory, see `INVENTORY.md`.

## What Stays In Manatuabon

The live Nemotron-backed observatory code remains in Manatuabon, especially the runtime client, bridge integration, ingest path, governance path, tests, and operational docs.

Those files are part of the current application contract and should not be moved into this archive repo. For the exact split, see `ACTIVE_VS_ARCHIVE.md`.

## External Assets Not Vendored Here

Large or environment-specific files were intentionally left out:

- submission ZIP archives
- LoRA weight binaries and checkpoint directories
- additional Drive-only notebook copies not imported here
- Colab runtime outputs and credentials files

See `EXTERNAL_IMPORT_CHECKLIST.md`, `DRIVE_LORA_MANIFEST.md`, and `SUBMISSION_HISTORY.md` for the recorded external trail.

## Why This Archive Exists

This challenge work is historically useful because it shows:
- how the synthetic reasoning datasets were generated
- how LoRA and QLoRA experiments were organized
- what was shipped as competition submissions
- which artifacts later influenced Manatuabon's local-model direction

It should be read as a lessons-learned engineering archive, not as the source of truth for the live observatory.