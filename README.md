# ROCS-Query-Prep-Benchmark

A curated collection and analysis of research on the impact of query preparation strategies in ROCS-based virtual screening.

## 📖 Background
ROCS (Rapid Overlay of Chemical Structures, by OpenEye) is a leading shape-based virtual screening tool widely used in drug discovery.  
While ROCS is powerful, its performance strongly depends on how the **query molecule(s)** are prepared.  
Key factors include:
- Choice of query conformation(s)
- Single vs. multiple conformers
- Query ensembles (multi-query strategies)
- Protonation states, tautomers, stereochemistry
- Inclusion and weighting of chemical features ("color" force field)

This project summarizes literature that evaluates these factors and provides guidance for best practices in ROCS-based workflows.

## 📚 Literature Summary
A collection of studies that specifically discuss the effect of query preparation on ROCS performance:

- **Tawa et al., 2009** – Effects of query conformations on ROCS screening outcomes.  
- **Langdon et al., 2013** – Role of conformer generation (OMEGA) and scaffold-focused screening.  
- **Liu et al., 2018** – Model selection and prospective screening considerations.  
- **Kearnes et al., 2016** – ROCS-derived features and chemical color weighting.  
- **Alexandrov et al., 2022** – Multi-query/ensemble strategies and chemical information inclusion.

(*More references will be added in `references.md`*)

## 🧪 Best Practices (from literature)
- Use multiple conformers of the query rather than relying on a single low-energy conformer.  
- Consider using crystallographic conformations when available.  
- Include multiple protonation states, stereoisomers, or tautomers when relevant.  
- Test both shape-only and shape+color modes; chemical feature weighting can change ranking.  
- Ensemble queries (multi-query consensus) often improve robustness and hit enrichment.  

## 📂 Repository Structure
```
ROCS-Query-Prep-Benchmark/
├── README.md # Project overview
├── references.md # Full bibliographic references
├── notes/ # Annotated reading notes for each paper
├── figures/ # Diagrams or comparison plots
└── data/ # Example query setups or benchmark results
```
