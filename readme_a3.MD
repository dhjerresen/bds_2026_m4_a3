# Assignment 3

## 📊 Comparative Analysis

| Model Version | Training Data Source | F1 Score (Eval Set) |
|---|---|---:|
| 1. Baseline | Frozen Embeddings (No Fine-tuning) | 0.7618 |
| 2. Assignment 2 Model | Fine-tuned on Silver + Gold (Simple LLM) | 0.8033 |
| 3. Assignment 3 Model | Fine-tuned on Silver + Gold (Agent Debate) | 0.8052 |

### Agreement with Human Labels

- Assignment 2 (Simple LLM → Human): **91%**
- Assignment 3 (Agent System → Human): **95%**

The agent-based workflow achieved higher agreement with human labels compared to the simple LLM approach.

### Reflection

The advanced agent-based workflow achieved slightly higher downstream model performance compared to the simple LLM approach (F1: 0.8033 → 0.8052) while also improving agreement with human labels (91% → 95%). This suggests that structured reasoning through multiple agents can improve label quality, particularly for borderline cases, although the overall downstream gain remains modest given the small number of additional labeled examples. The results indicate diminishing returns relative to the added system complexity.
