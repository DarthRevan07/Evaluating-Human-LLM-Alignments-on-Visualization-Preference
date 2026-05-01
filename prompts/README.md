# Data Generation Pipeline Prompts

This directory contains all prompts used in the data generation pipeline for the study **"Evaluating Human-LLM Alignments on Visualization Preference"**.

## Files

| File | Description |
|------|-------------|
| `data_generation_prompts.json` | Prompts used to generate visualization pair descriptions and metadata |
| `evaluation_prompts.json` | Prompts used to query LLMs for visualization preference judgments |

## Overview

The data generation pipeline consists of two stages:

1. **Visualization Pair Generation** (`data_generation_prompts.json`): We prompted LLMs to generate descriptions of visualization pairs across several design dimensions (chart type, color encoding, data-ink ratio, etc.). Each pair consists of a "base" visualization and an "alternative" visualization that differs along one or more design axes.

2. **LLM Preference Evaluation** (`evaluation_prompts.json`): These prompts were used to present each visualization pair to LLMs and collect their preference judgments, along with free-text rationales. The prompts were designed to mirror the instructions given to human annotators in the annotation study.
