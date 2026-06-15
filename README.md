# objetivos
- Construir un corpus de artículos sobre explicabilidad
- Generar embeddings semánticos
- Identificar clusters temáticos
- Analizar relaciones entre métodos
- Explorar conexiones con la propuesta geométrica de Jiang et al.

# Estructura
llm-explainability-mapping/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── embeddings/
│
├── notebooks/
│   ├── 01_explore_corpus.ipynb
│   ├── 02_generate_embeddings.ipynb
│   └── 03_clustering.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── embeddings.py
│   ├── clustering.py
│   └── visualization.py
│
├── results/
│   ├── figures/
│   ├── tables/
│   └── reports/
│
├── papers/
│   ├── pdfs/
│   └── bibliography.bib
│
└── docs/
    └── notes.md
# Primer experimento
- Generar embeddings de abstrcts usando Sentence-BERT y visualizar clusters mediante UMAP.

# Segundo experimento
ACL Anthology
↓
DataFrame
↓
Filtro interpretability/probing
↓
Embeddings
↓
UMAP
↓
Clusters
↓
Mapa conceptual del campo

La estructura que encontré en acl-anthology es:
collection
│
└── volume
     │
     ├── meta
     │
     ├── paper
     ├── paper
     ├── paper
     └── ...
## Corpus
### Test
Construiré un corpus con los archivos de meta análisis previos:
(Wallace et al., 2018; Pathologies of neural models make interpretations difficult
Ross et al., 2017)
(Alvarez-Melis and Jaakkola, 2017;
Poerner et al., 2018;
Ribeiro et al., 2016)
(Croce et al., 2018; 
<hasta aquí llegué y me cambie al de Calderon y Reichart>
Jiang et al., 2019)
(Mullenbach et al., 2018; 
Ghaeini et al., 2018; 
Xie et al., 2017; 
Aubakirova and Bansal, 2016)
(Ling et al., 2017; 
Dong et al., 2019; 
Pezeshkpour et al., 2019a)
(Abujabal et al., 2017)
(Rajani et al., 2019a;
Sydorova et al., 2019)
(Croce et al., 2019)
(Pryzant et al., 2018a,b)
(Liu et al., 2018)
(Pr¨ollochs et al., 2019)

<Calderon y Reichart>
Afra Amini, Tiago Pimente... 2023

Los almaceno todos en zotero.


### Búsqueda
1. Probing
2. Attention
3. Saliency
4. Mechanistic interpretability
5. Sparse autoencoders
6. Causal methods
7. Chain of thought explanations


### Lista
1. Bibal, Adrien, Rémi Cardon, David Alfter, et al. “Is Attention Explanation? An Introduction to the Debate.” Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), 2022, 3889–900. https://doi.org/10.18653/v1/2022.acl-long.269.
2. Hornischer, Levin, and Hannes Leitgeb. “Explaining Neural Networks with Reasons.” arXiv:2505.14424. Preprint, arXiv, May 21, 2025. https://doi.org/10.48550/arXiv.2505.14424.
3. Zytek, Alexandra, Sara Pidò, and Kalyan Veeramachaneni. “LLMs for XAI: Future Directions for Explaining Explanations.” arXiv:2405.06064. Preprint, arXiv, May 9, 2024. https://doi.org/10.48550/arXiv.2405.06064.
