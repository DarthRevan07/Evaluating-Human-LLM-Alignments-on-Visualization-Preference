# Evaluating Human-LLM Alignments on Visualization Preference

This repository houses the supplementary material for the submission **"Evaluating Human-LLM Alignments on Visualization Preference"** at IEEE VIS 2026 (Short Papers Track).

## Repository Structure

```
.
├── prompts/                        # Data generation pipeline prompts
│   ├── README.md
│   ├── data_generation_prompts.json   # Prompts used to generate visualization pair descriptions
│   └── evaluation_prompts.json        # Prompts used to query LLMs for preference judgments
│
├── model_responses/                # LLM model responses
│   ├── README.md
│   └── responses.json              # Full structured responses from all evaluated LLMs
│
└── supplementary_pdfs/             # PDF supplementary documents
    ├── README.md
    ├── annotation_ui_overview.pdf       # Overview of the annotation UI and study flow
    └── annotator_grading_samples.pdf    # Samples of annotator preference grading with human-LLM comparisons
```

## Contents

### `prompts/`
Contains all prompts used in the two-stage data generation pipeline:
- **`data_generation_prompts.json`** — Prompts that guided the creation of visualization pair descriptions across five design dimensions (chart type, color encoding, data-ink ratio, axis scale, annotation density).
- **`evaluation_prompts.json`** — Five prompt variants (zero-shot, criteria-guided, audience-aware, batch ranking, forced-choice) used to elicit LLM preference judgments on each visualization pair.

### `model_responses/`
Contains structured LLM responses collected during the preference evaluation stage:
- **`responses.json`** — Per-pair, per-model, per-prompt-condition response records including stated preference (A/B), free-text rationale, confidence level, and raw model output. Six models evaluated: GPT-4o, GPT-4 Turbo, Claude 3.5 Sonnet, Claude 3 Opus, Gemini 1.5 Pro, and Llama 3.1 70B.

### `supplementary_pdfs/`
PDF documents providing visual and descriptive overviews:
- **`annotation_ui_overview.pdf`** — Details the web-based annotation platform (technology stack, study flow, per-pair interface, quality-control measures, annotator demographics).
- **`annotator_grading_samples.pdf`** — Presents curated samples of human preference judgments for five representative pairs, with annotator rationale quotes and side-by-side human vs. LLM preference comparisons.

## Citation

If you use these materials, please cite:

```
@inproceedings{vis2026-human-llm-viz,
  title     = {Evaluating Human-LLM Alignments on Visualization Preference},
  booktitle = {IEEE VIS 2026 (Short Papers Track)},
  year      = {2026}
}
```
