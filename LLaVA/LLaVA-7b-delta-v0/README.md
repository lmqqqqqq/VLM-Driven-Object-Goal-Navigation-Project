---
license: apache-2.0
inference: false
---

**NOTE: This "delta model" cannot be used directly.**  
Users have to apply it on top of the original LLaMA weights to get actual LLaVA weights.  
See https://github.com/haotian-liu/LLaVA#llava-weights for instructions.

<br>
<br>

# LLaVA Model Card

## Model details

**Model type:**
LLaVA is an open-source chatbot trained by fine-tuning LLaMA/Vicuna on GPT-generated multimodal instruction-following data.
It is an auto-regressive language model, based on the transformer architecture.

**Model date:**
LLaVA was trained in April 2023.

**Paper or resources for more information:**
https://llava-vl.github.io/

**License:**
Apache License 2.0

**Where to send questions or comments about the model:**
https://github.com/haotian-liu/LLaVA/issues

## Intended use
**Primary intended uses:**
The primary use of LLaVA is research on large multimodal models and chatbots.

**Primary intended users:**
The primary intended users of the model are researchers and hobbyists in computer vision, natural language processing, machine learning, and artificial intelligence.

## Training dataset
595K filtered image-text pairs from CC3M.
150K GPT-generated multimodal instruction-following data.

## Evaluation dataset
A preliminary evaluation of the model quality is conducted by creating a set of 90 visual reasoning questions from 30 unique images randomly sampled from COCO val 2014 and each is associated with three types of questions: conversational, detailed description, and complex reasoning. We utilize GPT-4 to judge the model outputs.
We also evaluate our model on the ScienceQA dataset.  Our synergy with GPT-4 sets a new state-of-the-art on the dataset.
See https://llava-vl.github.io/ for more details.
