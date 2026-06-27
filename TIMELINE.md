# Timeline

## Phase 1: Competition Setup

- Challenge data and starter notebooks were gathered.
- Early workflow centered on Kaggle and notebook-driven iteration.
- Initial synthetic reasoning dataset generation was assembled.

## Phase 2: Training Data Refinement

- `kaggle_pipeline.py` generated synthetic training traces.
- `kaggle_ensemble_mix.py` merged legacy traces with newer reasoning examples.
- Training corpora such as `synthetic_cot.jsonl` and `master_ensemble_dataset.jsonl` became the backbone of the workflow.

## Phase 3: LoRA / QLoRA Iteration

- Colab notebooks were used to train and package Nemotron adapters.
- `submission.zip` through `submission15.zip` record repeated iteration on adapter packaging.
- Local and notebook-side inference/testing paths evolved in parallel.

## Phase 4: Local Experiment Extensions

- `nemotron_self_play_vllm.py` captured a more experimental local self-play path.
- Additional inference notebooks in Downloads preserved side branches of the competition workflow.

## Phase 5: Product Crossover

- Parts of the Nemotron effort influenced Manatuabon's local-model strategy.
- Runtime files such as the live Nemotron client, bridge integration, and governance paths stayed in the main application.
- The original challenge artifacts remained useful historically but no longer belonged in the same conceptual bucket as the observatory runtime.

## Phase 6: Historical Consolidation

- The challenge artifacts were staged into this standalone archive.
- Heavy binary submission artifacts were documented but not vendored into git.
- The archive was reframed as a lessons-learned engineering record.