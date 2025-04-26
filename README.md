# LLM Engineering - Experiments & Implementations

A comprehensive collection of AI/ML experiments and production-ready implementations exploring the full spectrum of modern LLM engineering - from foundational concepts to deploying autonomous multi-agent systems.

## 🎯 Key Skills Demonstrated

- **LLM Development**: Fine-tuning, prompt engineering, quantization (QLoRA), model deployment
- **RAG Systems**: Vector databases (ChromaDB), embeddings, semantic search, advanced retrieval techniques
- **Production ML**: Model deployment (Modal), API design, containerization, cloud infrastructure
- **Multi-Agent AI**: Autonomous agent orchestration, ensemble methods, real-time decision making
- **Full-Stack AI**: End-to-end applications with Gradio UIs, REST APIs, push notifications
- **Model Evaluation**: Performance metrics, A/B testing, ensemble optimization

## 📚 Experiments Overview

### [Week 1: AI Fundamentals & API Integration](week1/)
**Focus**: Foundation concepts and API interactions

- **[Day 1](week1/day1.ipynb)**: OpenAI API, chat completions, structured outputs with Pydantic
- **[Day 2](week1/day2.ipynb)**: Prompt engineering, function calling, JSON mode
- **[Day 3](week1/day3.ipynb)**: Image generation (DALL-E), vision models (GPT-4 Vision)
- **[Day 4](week1/day4.ipynb)**: Anthropic Claude API, content moderation
- **[Day 5](week1/day5.ipynb)**: Streaming responses, audio transcription (Whisper)

**Tech Stack**: OpenAI API, Anthropic API, Pydantic, JSON schemas

---

### [Week 2: LangChain & Agent Development](week2/)
**Focus**: Building chains and simple agents

- **[Day 1](week2/day1.ipynb)**: LangChain fundamentals, chains, templates
- **[Day 2](week2/day2.ipynb)**: Memory systems, conversation management
- **[Day 3](week2/day3.ipynb)**: Agent architectures, ReAct pattern, tool usage
- **[Day 4](week2/day4.ipynb)**: Multi-step reasoning, planning agents
- **[Day 5](week2/day5.ipynb)**: Custom tools, agent debugging

**Tech Stack**: LangChain, OpenAI, agent frameworks

---

### [Week 3: Local Models & HuggingFace](week3/)
**Focus**: Running models locally, understanding transformer architectures

- **[Day 1](week3/day1_colab_intro.ipynb)**: Google Colab setup, GPU utilization, Stable Diffusion XL, FLUX
- **[Day 2](week3/day2_huggingface_pipelines.ipynb)**: HuggingFace pipelines (sentiment, NER, QA, summarization, generation)
- **[Day 3](week3/day3_tokenizers.ipynb)**: Tokenizer deep-dive (Llama 3.1, Phi-4, DeepSeek, QwenCoder)
- **[Day 4](week3/day4_transformer_models.ipynb)**: Model architecture, quantization (4-bit, 8-bit), memory optimization
- **[Day 5](week3/day5_meeting_minutes.ipynb)**: Audio-to-text pipeline (Whisper + GPT for meeting summaries)

**Tech Stack**: HuggingFace Transformers, bitsandbytes, Stable Diffusion, FLUX, Whisper

---

### [Week 4: Advanced Code Generation](week4/)
**Focus**: Multi-language code generation and benchmarking

- **[Day 1](week4/day1.ipynb)**: Python optimization, code refactoring with LLMs
- **[Day 2](week4/day2.ipynb)**: Test generation, documentation automation
- **[Day 3](week4/day3.ipynb)**: Python → C++ translation, compilation, benchmarking
- **[Day 4](week4/day4.ipynb)**: Gradio UI for multi-model code generation comparison
- **[Day 5](week4/day5.ipynb)**: Python → Rust translation, advanced RAG (reranking, query rewriting)

**Tech Stack**: OpenAI, Anthropic, Gradio, C++/Rust compilers, RAG patterns

---

### [Week 5: RAG Systems - From Basic to Advanced](week5/)
**Focus**: Building production-grade retrieval systems

**Knowledge Base**: [76 documents](week5/knowledge-base/) (company, contracts, employees, products)

- **[Day 1](week5/day1.ipynb)**: Basic RAG with keyword matching, Gradio chat interface
- **[Day 2](week5/day2.ipynb)**: Vector embeddings (OpenAI), ChromaDB, semantic search, vector visualization
- **[Day 3](week5/day3.ipynb)**: LangChain integration, retriever patterns, temperature tuning
- **[Day 4](week5/day4.ipynb)**: RAG evaluation pipeline, test datasets ([tests.jsonl](week5/evaluation/tests.jsonl)), performance metrics
- **[Day 5](week5/day5.ipynb)**: Advanced RAG - LLM-enhanced chunking, reranking, query rewriting

**Implementation**: 
- [Basic](week5/implementation/) vs [Advanced](week5/pro_implementation/) implementations
- [Evaluation framework](week5/evaluation/) with 38K test cases

**Tech Stack**: LangChain, ChromaDB, OpenAI Embeddings, Pydantic, performance optimization

---

### [Week 6: Product Pricer - Complete ML Pipeline](week6/)
**Focus**: Fine-tuning LLMs for real-world pricing tasks

**Project**: E-commerce product price estimation (400K products, 8 categories)

- **[Day 1](week6/day1.ipynb)**: Data curation from Amazon reviews, prompt engineering for training
- **[Day 2](week6/day2.ipynb)**: Dataset scaling, HuggingFace Datasets, training/test splits
- **[Day 3](week6/day3.ipynb)**: Baseline ML models (Random Forest on word2vec embeddings)
- **[Day 4](week6/day4.ipynb)**: Frontier model benchmarking (GPT-4o-mini)
- **[Day 5](week6/day5.ipynb)**: OpenAI fine-tuning, Weights & Biases monitoring, model comparison

**Results**: Fine-tuned model achieves $76 avg error vs $396 base model, $127 human baseline

**Tech Stack**: OpenAI Fine-tuning API, W&B, HuggingFace Datasets, scikit-learn

---

### [Week 7: Open-Source Model Fine-Tuning](week7/)
**Focus**: Advanced fine-tuning with QLoRA on open-source models

**Project**: Product Pricer v2 - Llama 3.1 8B fine-tuning

- **[Day 1](week7/Week_7_Day_1_qlora_intro.ipynb)**: Quantization experiments (4-bit, 8-bit), QLoRA introduction
- **[Day 2](week7/Week_7_Day_2_base_model_evaluation.ipynb)**: Base model selection (Llama 3.1 8B), tokenizer comparison
- **[Day 3](week7/Week_7_Day_3_TRAINING.ipynb)**: QLoRA fine-tuning with W&B monitoring, LoRA configuration
- **[Day 5](week7/Week_7_Day_5_Testing_our_Fine_tuned_model.ipynb)**: Model evaluation, weighted token predictions

**Key Achievement**: Successfully fine-tuned 8B parameter model on consumer GPU using 4-bit quantization

**Tech Stack**: PyTorch, bitsandbytes, PEFT, QLoRA, Transformers, Weights & Biases

---

### [Week 8: Production Multi-Agent AI System](week8/) ⭐
**Focus**: Building and deploying autonomous agent frameworks

**Project**: "The Price is Right" - AI Deal-Hunting System

#### Architecture Overview
Multi-agent system that autonomously finds and evaluates online deals:

**Core Agents**:
- **[SpecialistAgent](week8/agents/specialist_agent.py)**: Fine-tuned Llama 3.1 8B (deployed on Modal)
- **[FrontierAgent](week8/agents/frontier_agent.py)**: RAG + GPT-4o-mini (ChromaDB vector search)
- **[RandomForestAgent](week8/agents/random_forest_agent.py)**: ML model on sentence embeddings
- **[EnsembleAgent](week8/agents/ensemble_agent.py)**: Weighted combination via Linear Regression

**Orchestration**:
- **[ScannerAgent](week8/agents/scanner_agent.py)**: RSS feed scraping, GPT-4o-mini parsing
- **[PlanningAgent](week8/agents/planning_agent.py)**: Coordinates all agents, opportunity detection
- **[MessagingAgent](week8/agents/messaging_agent.py)**: Push notifications (Pushover)

#### Daily Breakdown

- **[Day 1](week8/day1.ipynb)**: Modal deployment, serverless functions, agent basics
- **[Day 2.0](week8/day2.0.ipynb)**: Vector database creation (400K products → ChromaDB)
- **[Day 2.1](week8/day2.1.ipynb)**: 2D visualization (t-SNE)
- **[Day 2.2](week8/day2.2.ipynb)**: 3D visualization
- **[Day 2.3](week8/day2.3.ipynb)**: RAG pipeline with GPT-4o-mini, DeepSeek alternative
- **[Day 2.4](week8/day2.4.ipynb)**: Random Forest training, ensemble model optimization
- **[Day 3](week8/day3.ipynb)**: RSS feed scanning, deal selection with GPT-4o-mini
- **[Day 4](week8/day4.ipynb)**: Push notifications, planning agent coordination
- **[Day 5](week8/day5.ipynb)**: Gradio UI, complete system integration

#### [Complete Implementation: Autonomous Deal Hunter](week8/price_is_right_autonomous.ipynb)
End-to-end walkthrough covering:
- Modal deployment and authentication
- ChromaDB vector store population
- All agent implementations and testing
- Ensemble model training and evaluation
- Full system deployment with Gradio interface

**Key Features**:
- Autonomous 24/7 operation
- Multi-model ensemble for improved accuracy
- Real-time notifications
- Production-ready deployment on Modal
- Persistent memory system

**Tech Stack**: Modal, ChromaDB, SentenceTransformers, scikit-learn, Gradio, Pushover, RSS parsing

---

## 🛠️ Technologies & Frameworks

**LLM Platforms**: OpenAI (GPT-4, GPT-4o-mini), Anthropic (Claude), HuggingFace (Llama, Phi, DeepSeek, Qwen), DeepSeek API

**ML/DL**: PyTorch, Transformers, PEFT, QLoRA, bitsandbytes, scikit-learn, Random Forest

**Vector Databases**: ChromaDB, OpenAI Embeddings, SentenceTransformers

**Frameworks**: LangChain, LangGraph, Gradio, Pydantic, W&B

**Deployment**: Modal (serverless), Google Colab, REST APIs

**Tools**: Whisper, DALL-E, Stable Diffusion, FLUX, RSS parsing

---

## 📊 Key Projects Summary

| Project | Week | Technologies | Achievement |
|---------|------|--------------|-------------|
| **Meeting Minutes Generator** | 3 | Whisper, GPT-4 | Audio → Structured minutes |
| **Multi-Language Code Gen** | 4 | GPT-4, Claude, Gradio | Python → C++/Rust translation |
| **RAG System** | 5 | ChromaDB, LangChain | Advanced retrieval with reranking |
| **Product Pricer (OpenAI)** | 6 | Fine-tuning, W&B | $76 avg error (40% better than human) |
| **Product Pricer (QLoRA)** | 7 | Llama 3.1 8B, QLoRA | 8B params on consumer GPU |
| **Deal-Hunting AI** | 8 | Multi-agent, Modal | Production autonomous system |

---

## 💡 Skills Progression

**Weeks 1-2**: API integration, prompt engineering, basic agents  
**Weeks 3-4**: Local models, optimization, code generation  
**Weeks 5-6**: RAG systems, fine-tuning, production ML  
**Weeks 7-8**: Advanced fine-tuning, multi-agent systems, deployment

---

## 📂 Repository Structure

Each week contains:
- Jupyter notebooks with experiments and implementations
- Supporting Python modules and utilities
- Data/knowledge bases where applicable
- README documentation

---

## 🚀 Running the Projects

Most projects require:
```bash
pip install -r requirements.txt
```

Environment variables (create `.env` file):
```
OPENAI_API_KEY=your_key
ANTHROPIC_API_KEY=your_key
HF_TOKEN=your_token
```

For Week 8 deployment:
```bash
modal setup  # First time only
modal deploy -m week8/pricer_service2.py
```

---

**Note**: This repository documents hands-on exploration and experimentation with modern LLM engineering techniques, progressing from fundamental API usage to production-grade multi-agent systems deployed at scale.
