# 🧪 Rust + PumpFun Coding Assignment

## 📌 Objective
Build a small Rust program that ingests PumpFun token launch data, extracts meaningful behavioral signals, and produces a ranked list of tokens based on your scoring logic.  
This test evaluates your Rust fundamentals, async programming, data modeling, and reasoning skills.

---

## 📂 Assignment Overview

You will build a command-line Rust application that:

1. Fetches recent PumpFun token events (live API or mock JSON file).
2. Parses and deserializes the on-chain metadata.
3. Identifies wallet behavior patterns (repeat creators, snipers, early buyers, etc.).
4. Computes a score for each token based on your logic.
5. Outputs a ranked list of tokens with triggered signals.

Focus on code clarity, modular design, and correctness — not completeness or 100% accuracy.

---

## 🧱 Requirements

### 1. Language & Tooling
- Rust 1.74+
- Cargo project structure
- `tokio` for async runtime
- `serde` for data structures
- `reqwest` for HTTP (optional if using mock data)

---

## 2. Core Tasks

### **A. Data Ingestion**
Create an `ingest` module that retrieves PumpFun launches via one of:

#### **Option 1: Live API Pull (preferred)**
