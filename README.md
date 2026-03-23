# AI Adaptive Onboarding Engine

## Overview
The AI Adaptive Onboarding Engine is an intelligent skill-gap analysis and learning pathway generation system designed to optimize corporate onboarding experiences. By analyzing a candidate’s Resume alongside a target Job Description (JD), the system dynamically identifies missing competencies and constructs a personalized, dependency-aware learning roadmap.

Unlike traditional onboarding programs that follow static curricula, this solution enables adaptive skill progression, minimizing redundant training and accelerating role-specific readiness.

---

## Problem Statement
Modern corporate onboarding often adopts a “one-size-fits-all” learning approach, leading to:

- Experienced hires revisiting concepts they already know  
- Beginners struggling with advanced modules without proper foundations  
- Inefficient training time allocation and delayed productivity  

This project addresses these challenges by generating data-driven adaptive learning paths based on automated skill-gap analysis.

---

## Key Features
- ✅ Intelligent Resume & Job Description parsing  
- ✅ Rule-based NLP skill extraction engine  
- ✅ Automated skill-gap identification  
- ✅ Graph-based adaptive learning roadmap generation  
- ✅ Explainable recommendations (Reasoning Trace)  
- ✅ Functional web interface for document upload and visualization  
- ✅ Personalized training pathway sequencing  

---

## System Architecture
Resume PDF → Text Extraction → Skill Detection
JD PDF → Text Extraction → Required Skill Mapping
Skill Gap Engine → Dependency Graph → Roadmap Generator
Web UI Visualization

---

## Application Screenshots

### 🏠 Home — Resume & JD Upload
![Home UI](screenshots/ui_home.png)

### 📊 AI Insights Dashboard — Skill Gap Analysis
![Overview UI](screenshots/ui_overview.png)

### 🗺️ Personalized Learning Roadmap
![Roadmap UI](screenshots/ui_roadmap.png)

### 💡 Resume Rewrite + Smart Suggestions
![Suggestions UI](screenshots/ui_suggestions.png)

---

## Adaptive Pathing Logic:

The system models skill acquisition as a *dependency graph*, where advanced competencies require foundational prerequisites.

* Missing skills are identified via Resume–JD comparison
* Prerequisite chains are recursively expanded
* A topologically ordered roadmap is generated

### Example Learning Sequence:


Python → Machine Learning → Deep Learning

If Python is missing, the roadmap automatically begins with Python before progressing further.


## Tech Stack:

* *Python*
* *pdfplumber* (PDF text extraction)
* *Streamlit* (interactive web UI)
* Rule-based NLP skill matching engine
* Graph traversal logic (DFS-based adaptive sequencing)


## Datasets & Knowledge Sources:

* Kaggle Resume Dataset
* Job Description Dataset
* O*NET Skills Database

(All datasets are publicly available and used for skill reference modeling.)


## How to Run the Project:

### 1️⃣ Clone Repository

git clone https://github.com/madhav1431-create/Hackathon-Project.git
cd ai-adaptive-onboarding-engine

### 2️⃣ Install Dependencies

pip install -r requirements.txt

### 3️⃣ Launch Application

streamlit run app.py


## Sample Inputs:

Use the sample files provided in the repository:

* resume.pdf
* jd.pdf

Upload them via the web interface to generate a personalized roadmap.


## Expected Output:

* Detected resume competencies
* Required job skills
* Identified skill gaps
* Dependency-aware adaptive learning roadmap
* Explainable recommendation trace


## Demo Video:

 Add demo video link here


## Technical Presentation

Add presentation link here


## Future Improvements:

* Semantic skill understanding using LLM embeddings
* Knowledge tracing-based personalization
* Training duration estimation & difficulty scoring
* Real-time learner progress tracking
* Cross-domain onboarding generalization


## Contributors:

* Madhav Mittal
* Rishabh Shrivastava

---

## Hackathon Submission:

Developed as part of the *AI Adaptive Onboarding Engine Hackathon Challenge*, demonstrating intelligent skill-gap reasoning, adaptive curriculum sequencing, and practical onboarding optimization.
