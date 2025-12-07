---
layout: default
title: "Do Safety Circuits Transfer Across Languages ? Evidence of Safety Alignment Disparities between High- and Low-Resource Languages in LLMs "
Author: Chaymae Jaouhar
Completed: September 2025
---

# Do Safety Circuits Transfer Across Languages ? Evidence of Safety Alignment Disparities between High- and Low-Resource Languages in LLMs

<div style="text-align: right; margin-top: -20px; margin-bottom: 20px;">
  <a href="/research/CLA-figures" class="figures-button">Figures & Captions</a>
</div>

## Abstract
Large language models ( LLMs) are increasingly becoming a multilingual tool used by millions of people in a world with more than 7000 languages and different cultures. Yet, most alignment research, safety evaluation frameworks and mechanistic interpretability studies are influenced by underlying “assumptions” that are English language-dominated and despite notable efforts to empirically demonstrate the disparities in alignment across different languages, their internal representations remain under-explored. To address this gap, this work aims to study whether safety-related internal representations are weaker for low-resource languages than for high-resource languages, and whether they are structural and localized. The focus was on : English, French, Spanish, German, Arabic, Moroccan Darija, Tachelhit (Tamazight) and Afrikaans. The experiment provides insights into language-conditioned alignment in Gemma-2-2B-IT using Gemma Scope sparse autoencoders (SAEs) and a set of prompts limited to “safety” and “misinformation” themes due to compute constraints. Overall, the findings show tight clustering of stable safety features for high-resource languages while low-resource languages activate sparse features by comparing them across a diverse set of similarity metrics, and that the divergence is localized in mid-layers of the model. The findings highlight a critical safety divide : speakers of low-resource language may interact with significantly unsafe models. Ultimately, this work urges future research to develop multilingual alignment methods that generalize to multilingual contexts and ensure equitable safety across different linguistic communities. Through mechanistic interpretability, we can identify where the failures in safety circuits occur and how to enforce them.

## Keywords
Computation and Language, Mechanistic Interpretability, Cross-lingual Alignment, AI Safety, Model Evaluation, Sparse Autoencoders, Low-Resource Languages, High-Resource Languages, Language-Dependent Safety

## Full Research Manuscript & Code
For the complete paper, code, and additional project materials, please contact me.

*Notes: All experiments were conducted under modest compute resources with an emphasis on reproducibility, statistical robustness and transparency. 
The aim was to conduct "practical and pragmatic" experiments with a fast-feedback loop in alignment with the shifting trend in mechanistic interpretability towards "Method Minimalism".*
