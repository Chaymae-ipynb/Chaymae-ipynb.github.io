---
layout: default
title: "SHIFT (Supervised Hidden Internal Feature Tracing) - A Study of Representation Shift Under Supervision in LLMs"
Author: Chaymae Jaouhar
Completed: October 2025
---

# SHIFT - A Study of Representation Drift Under Supervision in LLMs

<div style="text-align: left; margin-top: -20px; margin-bottom: 20px;">
  <a href="/research/CS-figures" class="figures-button">Figures & Captions</a>
</div>

## Abstract
Large language models (LLMs) exhibit strong behavioral differences under supervised versus private prompt settings. The behavioral shift of LLMs under supervision can be seen as both a risk ( because models are vulnerable to adversarial attacks and their trustworthiness is unknown) and an opportunity ( because we can develop targeted safety alignment methods). This idea is dominating the general AI safety discourse where societal concerns about deceptive behavior and situational awareness are increasingly important. Prior research has shown that models condition their behavior on supervision signals in users’ prompts and are more vulnerable to jailbreak attacks when task framing is manipulated. However, the central focus has historically been the analysis of behavioral differences ( evaluating how outputs change under different modes) and less is known about how the supervision context is represented in the models’ hidden states and the extent to which the representations are stable and steerable. The aim of this study is to determine whether LLMs encode a linearly separable representation of “supervision” signals internally when being monitored vs unmonitored, and to localize and steer it mechanistically. Using a synthetic dataset of 30 jailbreak prompts, this work studies Gemma-2-2B-IT under a controlled two-mode setup ( evaluated versus private mode) and hidden states were extracted from two layers only ( 8 and 12) due to compute constraints. It introduces *SHIFT* ( Supervised Hidden Internal Feature Tracing), a two-stage experiment design that uses probing with layer-wise representation drift analysis and a trained sparse autoencoder (SAE), while mitigating the well-documented risks of the two methods. The findings reveal that the model forms a strong internal encoding of the supervision attribute with a high linear decodability especially at layer 12 and a directional drift that increases with layer depth as well. In the SAE stage, the experiment showed two main sparse features that align with this drift and steering them changed the generated text significantly. SHIFT exposes latent supervision awareness that is underexplored and unquantified in existing research which has significant implications for red-teaming, robustness against adversarial attacks and model alignment. Furthermore, *SHIFT* offers a light reproducible method to perform “cheap monitoring” and support future alignment methods by targeting internal representations rather than investing in intense reinforcement learning and fine-tuning methods.

## Keywords
Mechanistic Interpretability, AI Safety, Adversarial Attacks, LLM Jailbreaking, Large Language Models, Gemma Scope, Context Awareness, Activation Steering, Sparse Autoencoders, Linear Probes, Representation Drift

## Full Research Manuscript & Code
For the complete paper, code, and additional project materials, please contact me.

*Notes: All experiments were conducted under modest compute resources with an emphasis on reproducibility, statistical robustness and transparency. 
The aim was to conduct "practical and pragmatic" experiments with a fast-feedback loop in alignment with the shifting trend in mechanistic interpretability towards "Method Minimalism".*

