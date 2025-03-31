# Awesome-RL-based-LLM-Reasoning
[![PR Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/bruno686/Awesome-RL-based-LLM-Reasoning/pulls)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

# 📚 Paper Taxonomy

We categorize existing research by **data selection objectives** and **technical approaches**, with annotated summaries.  
*(Last Updated: {{DATE}})*  

---

## 1. 🔍 Data Quality Filtering  
**Goal**: Remove noisy/low-value data via quantitative metrics to improve training efficiency.

| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [Entropy Law: The Story Behind Data Compression and LLM Performance](#) | Data compression rate (entropy) as quality proxy | C4, Pile | High-compression data boosts performance (+12%) | [PDF](#) |
| [Less is More: Improving LLM Alignment via Preference Data Selection](#) | Reward model confidence filtering | Anthropic HH | 30% high-quality data achieves full-data performance | [Code](#) |
| [Principled Data Selection: The Hidden Risks of Difficult Examples](#) | Hard example distribution shift analysis | Reddit, StackExchange | Hard examples may harm OOD generalization | [PDF](#) |

---

## 2. 🌈 Data Diversity Optimization  
**Goal**: Balance data distribution to enhance generalization.

| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [Harnessing Diversity for Important Data Selection](#) | Embedding similarity-based sampling | The Pile | Improves cross-domain generalization (+8%) | [PDF](#) |
| [Adapt-∞: Dynamic Data Selection for Continual Learning](#) | Dynamic selection in continual learning | COCO, LAION | Reduces catastrophic forgetting (↓15%) | [Code](#) |

---

## 3. ⚖️ Alignment-Specific Selection  
**Goal**: Customize selection for safety/ethics/human preferences.

| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [SEAL: Safety-enhanced Aligned LLM Fine-tuning](#) | Toxicity scoring + safe data augmentation | ToxiGen | Reduces harmful outputs by 35% | [PDF](#) |
| [InCo-DPO: Balancing Distribution Shift and Data Quality](#) | Distributionally robust preference selection | UltraFeedback | Improves OOD robustness (+7%) | [Code](#) |

---

## 4. ⚡ Efficiency-Driven Methods  
**Goal**: Reduce computational cost of data selection.

| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [EDGE: Efficient Data Selection via Guideline Effectiveness](#) | Rule-based efficient filtering | Safe RLHF | 50% less data with 90% performance retained | [PDF](#) |
| [Dataset Decomposition: Variable-Length Curriculum Learning](#) | Sequence-length curriculum | C4 | 2x faster training | [Code](#) |

---

## 5. 📐 Theoretical Insights  
**Goal**: Fundamental principles and evaluation metrics.

| Title | Key Contribution | Resources |
|-------|------------------|-----------|
| [What Makes Good Data for Alignment?](#) | Defines "Informativeness-Diversity-Safety" triad | [PDF](#) |
| [Rethinking Data Shapley for Data Selection](#) | Improved Shapley value computation | [Code](#) |

---

## 🔎 Quick Lookup Table  
Find papers by technical keywords:

| Keyword | Related Papers |
|---------|----------------|
| **Entropy Filtering** | [Entropy Law](#), [Less is More](#) |
| **Distribution Robustness** | [InCo-DPO](#), [Distributionally Robust DPO](#) |
| **Multimodal Data** | [CLIPLoss](#), [Adapt-∞](#) |
| **Safety Alignment** | [SEAL](#), [Reward-Augmented Data](#) |

---

### How to Use
1. **Click titles** to jump to resources (replace `#` with actual links)
2. **Compare methods** within the same category (e.g., quality filtering techniques)
3. **Contribute**: Open an Issue/PR to add missing papers!

---

> ✨ **Pro Tip**: Use GitHub's table sorting plugins to dynamically reorder tables by columns like "Dataset" or "Key Findings".
