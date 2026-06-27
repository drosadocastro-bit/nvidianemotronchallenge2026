# Publishing Checklist

## Before First Push

1. Confirm no secrets are present.
2. Confirm `submission*.zip` files are still excluded.
3. Confirm no `.safetensors` or other large model binaries were copied in.
4. Review `downloads/` for anything that is too scratch-like to publish.
5. Add any Drive-only notebooks you still want preserved.

## Suggested First Commit Scope

Include:
- archive docs
- notebooks
- scripts
- training corpora that are already in this staging folder

Exclude:
- submission ZIP archives
- credentials
- heavyweight model files

## Good GitHub Framing

Suggested description:

`Historical archive of my NVIDIA Nemotron 2026 reasoning challenge workflow, including synthetic dataset generation, Colab training notebooks, inference experiments, and lessons learned.`

Suggested topics:

- `nvidia-nemotron`
- `kaggle`
- `llm-finetuning`
- `lora`
- `qlora`
- `colab`
- `reasoning`
- `historical-archive`

## Optional Follow-Up

1. Add a note describing how `submission.zip` changed over time.
2. Import any missing Google Drive notebook snapshots.
3. Add a short postmortem on what later fed into Manatuabon.