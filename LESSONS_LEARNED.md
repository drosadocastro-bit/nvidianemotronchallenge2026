# Lessons Learned

## What This Project Tried To Do

This work explored how to adapt NVIDIA Nemotron reasoning models for a competition workflow built around:
- synthetic chain-of-thought style data generation
- LoRA and QLoRA fine-tuning
- notebook-first experimentation in Kaggle and Colab
- repeated submission packaging through adapter checkpoints

## What Worked

- The project produced a reproducible synthetic data path through `kaggle_pipeline.py`.
- The ensemble merge step kept multiple reasoning styles available in a single training corpus.
- The submission process was disciplined enough to leave behind a sequence of archived adapter packages.
- The notebooks preserved the real competition workflow instead of hiding it behind a cleaned-up post hoc script.

## What Became Clear Midstream

- Notebook speed helped during the competition, but it scattered important context across Kaggle, Colab, Downloads, and local repo files.
- The submission ZIP history matters, but the raw binary payloads are not ideal for source control.
- Some Nemotron-related code inside Manatuabon stopped being competition code and became application runtime infrastructure.
- That split makes archive discipline important: historical training artifacts and live product code should not stay mixed forever.

## What This Archive Preserves Well

- training dataset generation
- training notebook flow
- inference notebook variants
- local self-play experimentation
- the existence of multiple submission iterations

## What Is Still Missing

- Google Drive-only notebooks not mounted on this machine
- any Colab-only outputs or notes that were never copied locally
- a textual summary of what changed from one submission ZIP to the next

## Main Engineering Lesson

Competition code can become product-adjacent very quickly. Once that happens, the codebase needs an explicit split between:
- historical experimentation worth preserving
- runtime code that now belongs to the live system

This archive is that split.