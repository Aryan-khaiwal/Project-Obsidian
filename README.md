# Project-Obsidian
Project Obsidian — Local LLM Prompt Structuring via QLoRA Fine-Tuning
## Problem Statement
Most users interact with online AI LLMs using vague, unstructured prompts, which leads to inconsistent and low-quality outputs. Writing high-quality prompts requires experience, structure, and time — a barrier for beginners and a friction point even for advanced users.
# Project Overview
Project Obsidian is a fully offline LLM system that takes a one-line user prompt and automatically expands it into a structured, high-quality prompt. The system removes the need for manual prompt engineering by learning prompt structure through fine-tuning on synthetic instruction data.
Pipeline Overview
15000 Synthetic instruction–response dataset generated from seed prompts
Base model - GPT-2 Large (774M) fine-tuned using QLoRA (4-bit) on local hardware rtx4050
Custom special tokens for instruction formatting
Deterministic JSON-only inference using brace-count parsing
Local inference with low latency (~1s on RTX 4050)
