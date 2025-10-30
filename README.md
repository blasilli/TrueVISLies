# Generative AI, Misleading Visualizations and their Rhetoric

This repository accompanies the paper 
> “_True (VIS) Lies: A Preliminary Analysis of How Generative AI is Capable of Recognizing Visualization Lies and their Rhetoric_” by Graziano Blasilli and Marco Angelili. 
Vis4GenAI - 1st Workshop on GenAI, Agents, and the Future of VIS https://visxgenai.github.io


## Abstract
This ongoing study analyzes the capability of multimodal Large Language Models (LLMs) to detect and interpret misleading data visualizations first, and then link them to root causes and intentionality using visualization rhetoric as a means to explain them. Three research questions are formulated and preliminarily analyzed experimentally using a dataset of 2,336 COVID-19-related tweets, half of which contain misleading visualizations using two models: Gemma3-27B and Qwen2.5-VL-72B. Results are additionally qualitatively evaluated on a small collection of ``real-life'' Vis Lies annotated by visualization researchers. The study's preliminary findings suggest that while these models have a baseline ability to detect visual deception, their effectiveness is highly dependent on the prompting strategy. Moreover, the results offer initial evidence that LLMs can begin to reason about the rhetorical dimension and intentionality of visual misinformation. The authors acknowledge the preliminary and non-generalizable nature of current findings, highlighting the need for further research.


## Contact
For any questions or further information, please contact:
- Graziano Blasilli: blasilli@diag.uniroma1.it
- Marco Angelili: angelini@diag.uniroma1.it



## Contents
- `/datasets` – Includes tweet IDs and metadata for misleading and non-misleading visualization samples.

- `experiments/` – Contains detailed model outputs for all experiments.

- `prompts/` – The exact prompts used in the experiments for reproducibility.

- `analysis/` – Scripts and notebooks for analyzing model outputs and generating results.
