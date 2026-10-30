# CDF-Eval: Conscience Diagnostic Framework Benchmark Engine

> **micro1 Frontier Engineering / Eval Submission** | A diagnostic LLM evaluation harness and vulnerability probe suite designed to detect unfaithful reasoning, narrative bias, sycophancy, and second-order risk blindness in frontier AI models.

---

## 🏗️ Baseline vs. Advanced Solution Architecture

| Architecture Tier | What It Does | Limitation / Bottleneck |
| :--- | :--- | :--- |
| **Baseline Solution** | Point-in-time pointwise LLM-as-a-judge scoring across standard static text prompts. | Suffers from subjective grader drift, prompt sensitivity, and unanchored hallucinations. |
| **Advanced Solution (v2.5)** | Hybrid execution engine combining Pydantic schemas, programmatic Regex exact-match anchors, Golden Reference grounding, and multi-model batch benchmarking. | Requires structured dataset curation and deterministic validation rules per probe. |

---

## 🚀 Quickstart & Reproduction Guide

### 1. Installation & Environment Setup
```bash
git clone [https://github.com/aldoriviano/cdf-eval.git](https://github.com/aldoriviano/cdf-eval.git)
cd cdf-eval
pip install -r requirements.txt
export OPENAI_API_KEY="your-openai-api-key"
