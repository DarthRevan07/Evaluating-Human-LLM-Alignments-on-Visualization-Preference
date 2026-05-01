# Model Responses

This directory contains raw LLM responses collected during the preference evaluation stage of the study **"Evaluating Human-LLM Alignments on Visualization Preference"**.

## Files

| File | Description |
|------|-------------|
| `responses.json` | Full structured responses from all LLMs across all visualization pairs and prompt conditions |

## Response Schema

Each entry in `responses.json` contains:

- `response_id` – Unique identifier for this response record  
- `pair_id` – Identifier of the visualization pair being evaluated  
- `model` – Name and version of the LLM that generated the response  
- `prompt_condition` – The evaluation prompt variant used (see `../prompts/evaluation_prompts.json`)  
- `preference` – The model's stated preference (`"A"` or `"B"`)  
- `rationale` – Free-text explanation provided by the model  
- `confidence` – Self-reported confidence level (`"Low"`, `"Medium"`, or `"High"`), where applicable  
- `raw_response` – The full unprocessed text output from the model  
- `timestamp` – ISO 8601 timestamp of when the response was collected  

## Models Evaluated

| Model | Provider | Version |
|-------|----------|---------|
| GPT-4o | OpenAI | gpt-4o-2024-05-13 |
| GPT-4 Turbo | OpenAI | gpt-4-turbo-2024-04-09 |
| Claude 3.5 Sonnet | Anthropic | claude-3-5-sonnet-20241022 |
| Claude 3 Opus | Anthropic | claude-3-opus-20240229 |
| Gemini 1.5 Pro | Google | gemini-1.5-pro-002 |
| Llama 3.1 70B | Meta | llama-3.1-70b-instruct |
