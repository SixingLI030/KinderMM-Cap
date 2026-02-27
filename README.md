# KinderMM-Cap: ECE Daily Activity Image Captioning

Official repository for the paper:

**Captioning Daily Activity Images in Early Childhood Education: Benchmark and Algorithm**

This repository provides the dataset, training framework, and model checkpoints for domain-specific image captioning in Early Childhood Education (ECE).

---

## 📌 Overview

Image captioning in Early Childhood Education (ECE) scenarios faces two major challenges:

1. **Lack of domain-specific large-scale datasets**, which limits fine-grained visual–semantic alignment and leads to generic object descriptions.
2. **Limitations of conventional training paradigms**, which struggle to enhance professional object description capability in specialized educational contexts.

To address these issues, we propose:

- **ECAC** — A large-scale benchmark dataset for ECE daily activity captioning.
- **RSRS** — A reward-conditional hybrid training framework integrating supervised fine-tuning and reinforcement learning.
- **KinderMM-Cap-3B** — A domain-adapted multimodal model trained with ECAC and RSRS.

---

## 📂 ECAC Dataset

**ECAC (Early Childhood Activity Captioning)** is a large-scale dataset specifically designed for ECE image captioning research.

### Dataset Features

- 256K+ real-world kindergarten daily activity images  
- Expert-level captions  
- Structured teaching toy annotations  
- Foreground/background object distinction  
- Multi-level naming precision labels  
- Domain-oriented evaluation metric (TTS)

### Directory Structure (Example)

ECAC/
├── images/
├── annotations/
│ ├── captions.json
│ ├── toy_labels.json
│ └── region_labels.json
└── splits/


### Download

- Dataset: *Coming Soon*
- Annotation Files: *Coming Soon*

---

## 🧠 RSRS Training Framework

**RSRS (Reward-Conditional Switch of Reinforcement Learning and Supervised Fine-Tuning)** is a dual-stream optimization framework designed for fine-grained object description tasks.

### Core Idea

- Apply reinforcement learning when reward signals are informative.
- Reroute zero-reward groups to supervised fine-tuning.
- Prevent advantage collapse in sparse-reward scenarios.
- Improve training stability and professional object recognition.

### Training Stages

1. **Stage 1: Domain-Specific Supervised Fine-Tuning (SFT)**
2. **Stage 2: Reward-Conditional Hybrid Optimization (RSRS)**

---

## 🤖 Model: KinderMM-Cap-3B

- Backbone: Qwen2.5-VL-3B
- Domain-adapted on ECAC
- Optimized with RSRS
- Enhanced professional teaching toy recognition

### Checkpoints

- Model weights: *Coming Soon*
- Inference config: *Coming Soon*

---

## 📊 Evaluation

We introduce **Teaching Toy Recognition Score (TTS)** to measure professional object naming accuracy in ECE scenarios.

Additional evaluation dimensions include:

- Scene recognition consistency  
- Human action description quality  
- Overall caption coherence  

---


