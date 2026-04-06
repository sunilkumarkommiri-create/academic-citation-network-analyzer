# Academic Citation Network Analyzer

## 📌 Overview
This project analyzes research papers by extracting citations and building a citation network graph.

## 🚀 Features
- Download papers from arXiv
- Extract text from PDFs
- Identify citations
- Build citation graph
- Semantic search using embeddings
- 
## 🏗️ System Architecture

The **Academic Citation Network Analyzer** follows a modular architecture that integrates external APIs, data processing, graph analysis, and visualization.

### 🔹 Architecture Overview

User Input → API Layer → Data Processing → Graph Construction → Analysis → Visualization

---

### 🔹 Components

#### 1. User Input Layer
- Accepts a research topic (e.g., "Machine Learning")
- Initiates the data pipeline

---

#### 2. API Layer (Semantic Scholar API)
- Searches for relevant research papers using query
- Fetches detailed metadata:
  - Paper title
  - Citations
  - References

---

#### 3. Data Processing Layer
- Cleans and filters API response
- Extracts required fields:
  - Paper IDs
  - Titles
  - Citation relationships

---

#### 4. Graph Construction Layer
- Uses NetworkX to build a **Directed Graph (DiGraph)**
- Nodes → Research Papers  
- Edges → Citation relationships  
  - A → B means A cites B

---

#### 5. Analysis Layer
- Computes graph metrics:
  - Degree Centrality
- Identifies:
  - Most influential papers
  - Highly connected nodes

---

#### 6. Visualization Layer
- Uses Matplotlib for graph visualization
- Displays citation network structure
- Spring layout for better node distribution

---


## 🛠️ Tech Used
- Python
- PyMuPDF
- NetworkX
- Sentence Transformers
- arXiv API

## ▶️ Run in Colab
Open the notebook and run all cells.

## 📊 Output
- Citation graph
- Influential papers
