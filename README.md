# IIT Indore AI Assistant – Query Preprocessing Engine

## 🚀 Overview

This project implements a **query preprocessing and expansion pipeline** for an AI assistant designed for IIT Indore.

It transforms raw, noisy user queries into **structured, semantically rich queries** optimized for retrieval systems (RAG pipelines).

---

## ✨ Features

* 🔍 Course code detection (e.g., CS204, EE460)
* 🧠 Jargon normalization (e.g., midsem → MSE)
* 🧾 Meaning-preserving query expansion
* 🔄 Multi-query generation using Groq (LLaMA models)
* ⚡ Modular and production-ready pipeline

---

## 🏗️ Pipeline

```text
User Query
   ↓
Cleaning
   ↓
Course Parsing
   ↓
Jargon Mapping
   ↓
Query Expansion
   ↓
Multi-query Generation
```

---

## 📦 Setup

```bash
git clone <repo_url>
cd IITI_BOT
pip install -r requirements.txt
```

Create `.env`:

```
GROQ_API_KEY=your_key_here
```

---

## ▶️ Run

```bash
python -m tests.run_tests
```

---

## 📌 Example

**Input:**

```
cs 204 midsem syllabus
```

**Output:**

```
CS204 MSE (mid semester examination) SYLLABUS
```

---

## 🎯 Goal

To bridge the gap between **student-style queries** and **structured academic knowledge retrieval**.

---

## 📄 Documentation

Detailed technical documentation is available in:

```
docs/PIPELINE.md
```
