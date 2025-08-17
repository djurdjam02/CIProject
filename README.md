# 🧬 CI Project – Genetic Algorithm for Missing Data Estimation in RCBD

## 📌 About the Project
This project implements a **Genetic Algorithm (GA)** to estimate missing values in **Randomized Complete Block Design (RCBD)** tables.  
RCBD is a commonly used statistical experimental design in agriculture, biology, and industry. However, missing data values often appear due to measurement errors or failed experiments, which disrupts analysis methods like ANOVA.  

To address this, we designed a GA-based method that imputes missing values while preserving the structure of RCBD experiments. Our approach was inspired by the work of Azadeh et al. (2012), but extended and improved with custom modifications and experiments.

---

## 🎯 Key Features
- Implementation of a **Genetic Algorithm** from scratch in Python.  
- Support for imputing **one or two missing values** in RCBD tables.  
- **Binary encoding of chromosomes** for efficient optimization.  
- **Fitness function based on SSE (Sum of Squared Errors)** for robust error minimization.  
- Genetic operators:
  - Roulette wheel selection
  - One-point and two-point crossover
  - Segment-based mutation  
- **Elitism** to preserve the best solutions across generations.  
- Experiments on both **synthetic and real-world data**.  
- Performance comparison with **existing literature implementations**.  

---

## 🚀 How It Works
1. Load an RCBD table (with one or two missing values).  
2. Encode missing values as chromosomes.  
3. Run the Genetic Algorithm with:
   - Initial random population
   - Fitness evaluation using SSE
   - Selection, crossover, and mutation  
4. Algorithm iterates through generations until convergence.  
5. The best individual (solution) represents the estimated missing value(s).  

---

## 📊 Results
- For **one missing value**, GA achieves near-perfect predictions (error < 1).  
- For **two missing values**, GA + derived formula yields stable and accurate imputations.  
- Comparison with literature shows **better or equal performance in most cases**.  
- Visualizations (fitness convergence, error metrics, histograms) confirm reliability.  

---

## 📖 References
- Azadeh, A., Ebrahimnejad, S., Saberi, M. (2013). *Optimum estimation of missing values in randomized complete block design by genetic algorithm*. Computers and Electronics in Agriculture, 93, 1-7.

---

## 👩‍💻 Authors
- **Dragana Katić** – 91/2021 Informatics, University of Belgrade  
- **Đurđa Milošević** – 84/2021 Informatics, University of Belgrade  

Mentorship: **Stefan Kapunac (Assistant), Vladimir Filipović (Professor)**  

---
