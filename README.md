# Vector embedding demos

A vector embedding encodes an input as a list of floating point numbers.

"dog" → [0.017198, -0.007493, -0.057982, 0.054051, -0.028336, 0.019245,…]

Different models output different embeddings, with varying lengths.

| Model | Encodes | Vector length |
| --- | --- | --- |
| word2vec | words | 300 |
| Sbert (Sentence-Transformers) | text (up to ~400 words) | 768 |
| OpenAI text-embedding-ada-002 | text (up to 8191 tokens) | 1536 |
| OpenAI text-embedding-3-small | text (up to 8191 tokens) | 256-1536 |
| OpenAI text-embedding-3-large | text (up to 8191 tokens) | 256-3072 |
| Azure AI Vision | image or text | 1024 |

Vector embeddings are commonly used for similarity search, fraud detection, recommendation systems, and RAG (Retrieval-Augmented Generation).

This repository contains a visual exploration of vectors, using several embedding models.

Before running the notebooks, install the requirements:

```shell
pip install -r requirements.txt
```

Then explore these notebooks:

* [Generate new OpenAI text embeddings](generate_embedding.ipynb)
* [Compare OpenAI and Word2Vec embeddings](comparison.ipynb)
* [Vector similarity](similarity.ipynb)
* [Vector search](search.ipynb)
* [Generate multimodal vectors for dataset](prep_multimodal.ipynb)
* [Explore multimodal vectors](multimodal_vectors.ipynb)
* [Vector distance metrics](distance_metrics.ipynb)
* [Vector quantization](quantization.ipynb)
* [Vector dimension reduction (MRL)](dimension_reduction.ipynb)

These notebooks are also provided, but aren't necessary unless you're generating new embeddings data.

* [Generate OpenAI embeddings for datasets](prep_openai.ipynb)
* [Generate Word2Vec embeddings for datasets](prep_word2vec_gnews.ipynb)
