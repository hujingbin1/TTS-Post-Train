# TTS-Post-Train

Static demo page for **Rethinking Post-Training for Expressive Zero-Shot Text-to-Speech**.

## Run locally

```bash
python3 -m http.server 8000
```

Open http://localhost:8000 in a browser. The page must be served over HTTP so the audio files load correctly.

## Included samples

The package contains the 30 samples shown by the page:

- 10 expressive cases
- 10 English cases
- 10 Chinese cases
- Reference audio plus Qwen3-TTS, Stage 1 Exp 0/1/2, GSPO (Stage 2), and OPSD (Stage 3)

The audio paths under `extracted/audio/` mirror the paths used by `demo-data.js`; no extra source dataset is required.

## Audio directory mapping

Each language directory uses the same paper-aligned names:

| Folder | Page label |
| --- | --- |
| `reference` | Reference |
| `qwen3-tts` | Qwen3-TTS |
| `stage1-exp0-sft` | SFT (Stage 1 Exp 0) |
| `stage1-exp1-dpo` | DPO (Stage 1 Exp 1) |
| `stage1-exp2-dpo` | DPO (Stage 1 Exp 2) |
| `stage2-gspo` | GSPO (Stage 2) |
| `stage3-opsd` | OPSD (Stage 3) |
