# Neural Machine Translation Codebase

This folder contains the source code and submitted outputs for the neural machine translation component of the NLP project.

## Structure

```text
part1/      BiLSTM encoder-decoder model with dot-product/global attention
part2/      Decoder-only Transformer with multi-head self-attention and causal masking
part3/      Attention heatmaps used for qualitative analysis
outputs/    Submitted JSON result files containing BLEU scores and generated translations
```

## Key Scripts

- `vocab.py` builds the source and target vocabularies/tokenizers.
- `train.py` trains the model and logs training progress to Weights & Biases when configured.
- `test.py` evaluates a trained model using BLEU.
- `predict.py` generates translations from a trained model checkpoint.
- `sanity_check.py` verifies core model components before training.

## Notes

Generated folders and files such as `.venv/`, `multi30k_data/`, `models/`, `vocab/`, `wandb/`, optimizer states, and model checkpoints are not included in this GitHub version. They can be regenerated during setup/training and are excluded to keep the repository clean and safe for public sharing.

Any Weights & Biases API keys must be provided by the user locally and should never be committed to GitHub.
