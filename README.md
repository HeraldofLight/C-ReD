# C-ReD: A Comprehensive Chinese Benchmark for AI-Generated Text Detection Derived from Real-World Prompts

Recently, large language models (LLMs) are capable of generating highly fluent textual content. While they offer significant convenience to humans, they also introduce various risks, like phishing and academic dishonesty. Numerous research efforts have been dedicated to developing algorithms for detecting AI-generated text and constructing relevant datasets. However, in the domain of Chinese corpora, challenges remain, including limited model diversity and data homogeneity. To address these issues, we propose **C-ReD**: a comprehensive **C**hinese **Re**al-prompt AI-generated **D**etection benchmark. Experiments demonstrate that C-ReD not only enables reliable in-domain detection but also supports strong generalization to unseen LLMs and external Chinese datasets-addressing critical gaps in model diversity, domain coverage, and prompt realism that have limited prior Chinese detection benchmarks.

[📄 Paper](https://arxiv.org/abs/2604.11796)  [💻 Dataset](https://github.com/HeraldofLight/C-ReD)
---

## 🔥 Overview
![Framework](figures/framework.png)
C-ReD is a large-scale **Chinese benchmark dataset for AI-generated text detection**, designed to evaluate model robustness across:

- Multiple **domains** (News, Q&A, Film Review, Academic Writing, Composition)
- Multiple **LLMs** (ChatGPT, Qwen, DeepSeek, Claude, etc.)
- Multiple **real-world prompt types**
- Both **in-domain and out-of-domain evaluation settings**

Unlike prior datasets, C-ReD emphasizes:

- 🧠 Real-world prompt simulation  
- 🌐 Strong generator diversity (including Chinese LLMs)  
- 📚 Multi-domain realistic text distribution  
- 🔄 Cross-domain & cross-model generalization  

---

## 📊 Dataset Statistics

- **Total samples:** 128,610  
  - Human-written: 12,997  
  - AI-generated: 115,613  
- **Domains:** 5 core domains 
- **Generators:** 9 state-of-the-art LLMs  
- **Unified schema across all samples**
 ### Example Schema

```json
{
  "id": 1,
  "text": "...",
  "label": 0,
  "domain": "news",
  "generator": "GPT-4o",
  "prompt": "...",
  "length": 512
}
