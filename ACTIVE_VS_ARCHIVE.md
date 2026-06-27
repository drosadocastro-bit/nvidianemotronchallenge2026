# Active Vs Archive Split

## Keep In Manatuabon

These are part of the live observatory runtime or its test/documentation surface:

- `manatuabon/core/nemotron_client.py`
- `manatuabon/core/ingest_agent.py`
- `manatuabon/core/consolidate_agent.py`
- `manatuabon/bridge/manatuabon_bridge.py`
- `manatuabon/governance/hypothesis_council.py`
- `manatuabon/workers/wiki_synthesis_worker.py`
- `tests/test_nemotron_client.py`
- runtime docs such as `README.md`, `SETUP.md`, and `WALKTHROUGH.md`

Reason:
These files are not just challenge remnants. They are the current Nemotron-backed operational path for query, chat, ingest, governance, or documentation.

## Safe To Archive Out Separately

These are historical competition or training artifacts:

- `kaggle_pipeline.py`
- `kaggle_ensemble_mix.py`
- `nemotron_self_play_vllm.py`
- `nvidia-nemotron-submission-demo.ipynb`
- `train_lora_colab.ipynb`
- `train_manatuabon_qlora_colab.ipynb`
- `synthetic_cot.jsonl`
- `synthetic_cot_grandmaster.jsonl`
- `master_ensemble_dataset.jsonl`
- the Downloads inference notebooks
- the submission ZIP history

Reason:
These files describe the competition workflow, training data generation, LoRA packaging, and notebook experimentation. They are historically valuable, but they are not part of the current observatory runtime contract.

## Ambiguous But Better In The Archive

- `train_manatuabon_qlora_colab.ipynb`

Reason:
It touches the broader Manatuabon direction, but its form is still a training notebook rather than live runtime logic. It fits better as an archive artifact with a note explaining that it bridges competition experimentation and later system work.