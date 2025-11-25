# EmbeddingClusteringVectorizationWorkshop

## Word Embeddings, Clustering, and Vectorization Workshop
**Course:** PROG8245  

---

## Team Members

| Team Member | Student ID |
|------------|------------|
| Oluwafemi Lawal | 8967308 |
| Jatinder Pal Singh | 9083762 |

---

## Dataset Description

### GloVe 6B Pre-trained Word Embeddings

This workshop uses the **Stanford GloVe** (Global Vectors for Word Representation) pre-trained embeddings.

#### Key Statistics (According to https://zenodo.org/records/4925376)
- **File Used:** `glove.6B.50d.txt` (50-dimensional vectors)
- **Training Corpus:** Wikipedia 2014 + Gigaword 5
- **Corpus Size:** ~6 billion tokens
- **Vocabulary Size:** 400,000 words
- **Dimension:** 50d 

#### Additional Corpora in Demo
| Corpus | Purpose |
|--------|---------|
| Sample NLP Text | Word2Vec training demonstration |
| Brown Corpus (NLTK) | Hierarchical clustering demonstration |

---

## 🔗 Dataset Source

**Source:** [Stanford NLP - GloVe](https://nlp.stanford.edu/projects/glove/)
- **Download:** http://nlp.stanford.edu/data/glove.6B.zip or https://zenodo.org/records/4925376
- **License:** [Public Domain Dedication and License (PDDL)](https://opendatacommons.org/licenses/pddl/)
- **Citation:** 
> Jeffrey Pennington, Richard Socher, and Christopher D. Manning. 2014. [GloVe: Global Vectors for Word Representation.](https://nlp.stanford.edu/pubs/glove.pdf)

> Riley Carlson, John Bauer, and Christopher D. Manning. 2025. [A New Pair of GloVes.](https://nlp.stanford.edu/pubs/glove.pdf)

---

## Workshop Contents

### Notebook: `EmbeddingClusteringVectorizationWorkshop_Fall2025.ipynb`

#### Part 1: Tutorial Demonstrations
- **Word2Vec Introduction:** CBOW and Skip-gram architectures
- **Word Similarity:** Finding semantically similar words
- **Brown Corpus Clustering:** Hierarchical clustering using co-occurrence
- **GloVe Introduction:** Loading and using pre-trained embeddings

#### Part 2: Workshop Analysis & Talking Points
- Demo summary with explanations
- Comprehensive Word2Vec vs GloVe comparison table
- Discussion of preprocessing, hyperparameters, and evaluation
- Key takeaways and recommendations

---

## Key Findings

### Word2Vec vs GloVe Comparison

| Aspect | Word2Vec | GloVe |
|--------|----------|-------|
| **Approach** | Predictive (neural network) | Count-based (matrix factorization) |
| **Training** | Local context window | Global co-occurrence statistics |
| **Best For** | Domain-specific training | General NLP with pre-trained vectors |
| **Speed** | Faster for small corpora | Faster for large corpora after matrix built |

### Key Talking Points
1. **Tokenization is foundational** - affects vocabulary and downstream quality
2. **Skip-gram vs CBOW** - Skip-gram better for rare words, CBOW faster for frequent words
3. **Pre-trained embeddings** - GloVe 6B captures general semantics from 6B tokens
4. **OOV Problem** - Neither handles unseen words (consider FastText or BERT)
5. **Bias awareness** - Pre-trained embeddings may encode societal biases

---

## License

This project is for educational purposes as part of PROG8245 coursework.

- **Code:** MIT License
- **GloVe Embeddings:** [Public Domain Dedication and License (PDDL)](https://opendatacommons.org/licenses/pddl/)
- **Brown Corpus:** Public Domain (via NLTK)
