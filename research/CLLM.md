---
layout: default
title: "When Models Fail to Use their Knowledge : Evidence of Behavior-Representation Divergence and Unsafe Biases in Clinical LLMs"
Author: Chaymae Jaouhar
Completed: November 2025
---

# When Models Fail to Use their Knowledge : Evidence of Behavior-Representation Divergence and Unsafe Biases in Clinical LLMs

## Abstract
Large Language Models (LLMs) are increasingly and routinely used in clinical recommendations, despite well-recognized risks. The field of AI safety has established that LLMs can make unsafe medical assumptions.Yet, the field shows little evidence on whether models incorporate safety-critical attributes ( i.e. age, pregnancy…) reliably into their internal representations, how they generate medical recommendations in under-specified user context and if they are based on hallucinated demographics. This paper aims to address this gap by presenting a new evaluation paradigm for AI safety in clinical LLMs and investigate whether steering attribute directions can mitigate unsafe behavior without using fine-tuning techniques.It introduces a contrastive evaluation of Gemma-2-2B-IT, using 20 synthetic clinical vignettes with each forming a triplet forming a total of 60 : user attribute is present/ absent/ under-specified ( the latter being the main focus of the study). The prompts follow the USMLE template. The experiment combines a detailed, simple and explainable text-level similarity analysis, hidden-state analysis and representation steering. The combination aims to isolate three levels of analysis : Behavior, Representations, Causality.The study shows that the model internally encodes safety-related attributes but does not reflect them in text generation, even when explicitly provided. Overall, in all 20 scenarios, the model defaults and assumes the low-risk attributes ( i.e. user is young, not pregnant…) when the attribute was not given in the input. The experiment also showed that some attributes are more linear and steerable than others. Additionally, explicitly including the attribute minimally influences the model’s generated text ( with a mean semantic difference of 0.1) and recommendations changed only 14% of the time). The paper offers novel insights as well as a practical and “pragmatic” evaluation design of “behavior-representation” divergence in LLMs. Furthermore, it argues that AI safety evaluation in the healthcare context should measure latent representations and outputs ( text-level evaluation).

## Keywords
AI Safety, AI Medical Reasoning, Explainable AI, Clinical Prompts, Model Evaluation, Mechanistic Interpretability, Gemma Scope, Clinical LLMs, Large Language Models, Medical Guideline Compliance

## Full Research Manuscript & Code
For the complete paper, code, and additional project materials, please contact me.

*Notes: All experiments were conducted under modest compute resources with an emphasis on reproducibility, statistical robustness and transparency. 
The aim was to conduct "practical and pragmatic" experiments with a fast-feedback loop in alignment with the shifting trend in mechanistic interpretability towards "Method Minimalism".*
