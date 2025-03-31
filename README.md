# Awesome Data Selection for LLM Alignment
[![PR Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/yimutianyang/Awesome-Data-Selection-for-LLM-Alignment)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)


# 📚 Paper Taxonomy

## 1. 🔍 Data Quality Filtering  
| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [Entropy Law: The Story Behind Data Compression and LLM Performance](https://arxiv.org/pdf/2407.06645) | Data compression rate (entropy) as quality proxy | C4, Pile | High-compression data boosts performance (+12%) | [PDF](https://arxiv.org/pdf/2407.06645) [Code](https://github.com/USTC-StarTeam/ZIP)|
| [Less is More: Improving LLM Alignment via Preference Data Selection](https://arxiv.org/abs/2502.14560) | Reward model confidence filtering | Anthropic HH | 30% high-quality data achieves full-data performance | [PDF](https://arxiv.org/abs/2502.14560)|
| [Principled Data Selection: The Hidden Risks of Difficult Examples](https://arxiv.org/abs/2502.09650) | Hard example distribution shift analysis | Reddit, StackExchange | Hard examples may harm OOD generalization | [PDF](https://arxiv.org/abs/2502.09650) [Code](https://github.com/glorgao/SelectiveDPO)|

## 2. 🌈 Data Diversity Optimization  
| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [Harnessing Diversity for Important Data Selection](https://openreview.net/forum?id=bMC1t7eLRc) | Embedding similarity-based sampling | The Pile | Improves cross-domain generalization (+8%) | [PDF](https://openreview.net/forum?id=bMC1t7eLRc)|
| [Adapt-∞: Dynamic Data Selection for Continual Learning](https://arxiv.org/pdf/2410.10636) | Dynamic selection in continual learning | COCO, LAION | Reduces catastrophic forgetting (↓15%) | [PDF](https://arxiv.org/pdf/2410.10636) [Code](https://github.com/adymaharana/adapt-inf) |

## 3. ⚖️ Alignment-Specific Selection  
| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [SEAL: Safety-enhanced Aligned LLM Fine-tuning](https://huggingface.co/papers/2408.02085) | Toxicity scoring + safe data augmentation | ToxiGen | Reduces harmful outputs by 35% | [PDF](https://arxiv.org/pdf/2408.02085) |
| [InCo-DPO: Balancing Distribution Shift and Data Quality](https://arxiv.org/pdf/2406.14115) | Distributionally robust preference selection | UltraFeedback | Improves OOD robustness (+7%) | [PDF](https://arxiv.org/pdf/2406.14115) [Code](https://github.com/alon-albalak/data-selection-survey) |

## 4. ⚡ Efficiency-Driven Methods  
| Title | Method | Dataset | Key Findings | Resources |
|-------|--------|---------|--------------|-----------|
| [EDGE: Efficient Data Selection via Guideline Effectiveness](https://arxiv.org/pdf/2402.05123) | Rule-based efficient filtering | Safe RLHF | 50% less data with 90% performance retained | [PDF](https://arxiv.org/pdf/2402.05123) |
| [Dataset Decomposition: Variable-Length Curriculum Learning](https://www.cs.princeton.edu/~smalladi/blog/2024/04/04/dataselection/) | Sequence-length curriculum | C4 | 2x faster training | [Code](https://github.com/princeton-nlp/LESS) |

## 5. 📐 Theoretical Insights  
| Title | Key Contribution | Resources |
|-------|------------------|-----------|
| [What Makes Good Data for Alignment?](https://arxiv.org/pdf/2408.02085) | Defines "Informativeness-Diversity-Safety" triad | [PDF](https://arxiv.org/pdf/2408.02085) |
| [Rethinking Data Shapley for Data Selection](https://openreview.net/pdf?id=hTBD3LYoqd) | Improved Shapley value computation | [PDF](https://openreview.net/pdf?id=hTBD3LYoqd) |
