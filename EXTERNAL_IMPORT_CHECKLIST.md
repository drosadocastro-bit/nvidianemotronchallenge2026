# External Import Checklist

## Downloads To Review Before Publishing

Bring these in only if you want a fuller historical record:

1. `submission.zip` through `submission15.zip`
2. `nvidia-nemotron-model-reasoning-challenge.zip`
3. any README or notes that explain why each submission changed

Recommendation:
- do not commit the raw submission ZIPs to git
- instead extract one representative folder structure or document the sequence in markdown
- if the adapter configs differ across submissions, preserve those diffs in text form

## Google Drive / Colab Imports

Imported from the mounted Drive already:

1. Nemotron Colab notebooks from `G:\My Drive\Colab Notebooks`
2. lightweight adapter metadata from `G:\My Drive\nemotron_reasoning_lora`

Still worth checking for additional imports:

1. intermediate Colab notebooks not already present here
2. training logs or screenshots that explain failed or successful runs
3. alternate dataset snapshots
4. exported adapter config variants not already represented
5. markdown notes or TODO files that explain parameter sweeps

Suggested import rule:
- keep notebooks, markdown notes, small JSON, and small CSV files
- exclude credentials, API keys, mounted-drive secrets, and large binary weights

Mounted heavy artifacts intentionally not imported:

1. `adapter_model.safetensors`
2. `tokenizer.json`
3. checkpoint directories under `G:\My Drive\nemotron_reasoning_lora`

## Secrets To Exclude

Never publish:

1. `kaggle.json`
2. OAuth tokens
3. Google Drive credentials
4. Colab secrets or environment exports

## If You Want A Strong Historical Repo

Add these before publishing:

1. a short timeline of the competition iterations
2. notes about what changed between submission ZIPs
3. a lessons-learned file on dataset generation, LoRA behavior, and inference constraints
4. any Drive-only notebook that captures a real experimental branch not already preserved here