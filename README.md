# ZeroGPU vs OpenAI Cost Calculator

A simple cost calculator that compares **OpenAI** API pricing with **ZeroGPU** for a given monthly token usage.

## What it does

- **Your usage:** Enter monthly input tokens and output tokens.
- **OpenAI:** Pick a model (GPT-5.4, GPT-5 mini, GPT-4.1, GPT-4.1 mini, GPT-4.1 nano). Uses current public pricing per 1M tokens.
- **ZeroGPU:** Pick a model (zlm-v1-summary-cloud, zlm-v1-iab-classify-cloud, nli-deberta-v3-small, t5-small-q8-v2). All use **$0.20/1M input**, **$0.40/1M output**. The calculator shows side‑by‑side cost and how much you’d save vs OpenAI.

## How to run

No build step. Open the HTML file in a browser:

```bash
open "ZeroGPU Calculator/index.html"
```

Or serve the folder with any static server (e.g. `npx serve "ZeroGPU Calculator"`) and open the URL.

## Notes

- OpenAI prices are from [openai.com/api/pricing](https://openai.com/api/pricing).
- ZeroGPU rates above are the current listed pricing for the small-models-edge family (summarization, IAB classification, NLI, etc.).
