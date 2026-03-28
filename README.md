# 日本語テキスト埋め込みモデル ベンチマーク

## データセット

### 尼崎市 Q&A データセット

京都大学が公開している BERT-Based FAQ Retrieval 用データセットを使用しています。

- [BERT-Based FAQ Retrieval (京都大学)](https://nlp.ist.i.kyoto-u.ac.jp/EN/index.php?BERT-Based_FAQ_Retrieval)
- [GitHub リポジトリ](https://github.com/ku-nlp/bert-based-faqir)

| 項目 | 内容 |
|------|------|
| コーパス | 尼崎市の Q&A ドキュメント 1,785 件 |
| クエリ | 検索クエリ 748 件 |
| 適合性判定 (qrels) | クエリとドキュメントのペアに対する関連度スコア (1: やや関連, 2: 高関連) |

## ベンチマーク

### Recall@10

| Rank | Publisher | Model | Score |
|------|-----------|-------|-------|
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 0.8231 |
| 2 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) | 0.8209 |
| 3 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) | 0.8136 |
| 4 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) | 0.8059 |
| 5 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 0.8016 |
| 6 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) | 0.8015 |
| 7 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.7922 |
| 8 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.7799 |
| 9 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) | 0.7778 |
| 10 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) | 0.7734 |
| 11 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) | 0.7654 |
| 12 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 0.7647 |
| 13 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) | 0.7622 |
| 14 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.7562 |
| 15 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.7478 |
| 16 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 0.7399 |
| 17 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.7383 |
| 18 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.7352 |
| 19 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 0.7342 |
| 20 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.7193 |
| 21 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.7155 |
| 22 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) | 0.7103 |
| 23 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.7058 |
| 24 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.6978 |
| 25 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.6819 |
| 26 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6730 |
| 27 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.6641 |
| 28 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.6595 |
| 29 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.6454 |
| 30 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.6416 |
| 31 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.6152 |
| 32 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) | 0.6000 |
| 33 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 0.5656 |
| 34 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) | 0.2471 |
| 35 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.1988 |
| 36 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.1798 |
| 37 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.1334 |
| 38 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.1298 |

### Precision@10

| Rank | Publisher | Model | Score |
|------|-----------|-------|-------|
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 0.1884 |
| 2 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) | 0.1868 |
| 3 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) | 0.1852 |
| 4 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) | 0.1850 |
| 5 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.1826 |
| 6 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) | 0.1817 |
| 7 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.1814 |
| 8 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 0.1777 |
| 9 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) | 0.1770 |
| 10 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) | 0.1768 |
| 11 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.1744 |
| 12 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) | 0.1744 |
| 13 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.1736 |
| 14 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) | 0.1721 |
| 15 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 0.1720 |
| 16 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 0.1698 |
| 17 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.1696 |
| 18 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.1684 |
| 19 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.1670 |
| 20 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) | 0.1634 |
| 21 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.1630 |
| 22 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.1628 |
| 23 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 0.1622 |
| 24 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.1586 |
| 25 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.1577 |
| 26 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.1526 |
| 27 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.1517 |
| 28 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.1514 |
| 29 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.1483 |
| 30 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.1479 |
| 31 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.1418 |
| 32 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) | 0.1368 |
| 33 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 0.1210 |
| 34 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) | 0.0563 |
| 35 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.0421 |
| 36 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.0378 |
| 37 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.0318 |
| 38 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.0215 |

### nDCG@10

| Rank | Publisher | Model | Score |
|------|-----------|-------|-------|
| 1 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) | 0.7255 |
| 2 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 0.7083 |
| 3 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) | 0.7069 |
| 4 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 0.6956 |
| 5 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) | 0.6908 |
| 6 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) | 0.6806 |
| 7 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.6662 |
| 8 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6657 |
| 9 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 0.6634 |
| 10 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) | 0.6590 |
| 11 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) | 0.6523 |
| 12 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) | 0.6492 |
| 13 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) | 0.6329 |
| 14 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.6278 |
| 15 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.6255 |
| 16 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.6206 |
| 17 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.6199 |
| 18 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 0.6176 |
| 19 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 0.6118 |
| 20 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.6004 |
| 21 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.5969 |
| 22 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) | 0.5897 |
| 23 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.5895 |
| 24 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.5858 |
| 25 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.5713 |
| 26 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.5628 |
| 27 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.5563 |
| 28 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.5553 |
| 29 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.5225 |
| 30 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.5211 |
| 31 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) | 0.4947 |
| 32 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) | 0.4939 |
| 33 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 0.4857 |
| 34 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) | 0.1879 |
| 35 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.1696 |
| 36 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.1275 |
| 37 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.1105 |
| 38 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.0876 |

## 評価方法

### 埋め込みの生成

各モデルを使用して、コーパス (ドキュメント) とクエリのテキストをベクトルに変換します。モデルによっては、クエリとドキュメントで異なるプレフィックスや `input_type` パラメータを指定しています。

### 検索 (Retrieval)

Elasticsearch の kNN (k-Nearest Neighbors) 検索を使用しています。

| 項目 | 設定値 |
|------|--------|
| 類似度関数 | コサイン類似度 |
| インデックスアルゴリズム | HNSW (Hierarchical Navigable Small World) |
| HNSW パラメータ | m=32, ef_construction=128 |
| 検索候補数 | 1,000 (num_candidates) |
| 取得件数 | 上位 100 件 |

各クエリのベクトルに対して、コーパス内のベクトルとのコサイン類似度が高い上位 100 件のドキュメントを取得し、その結果を評価メトリクスで評価します。

### 評価メトリクス

すべてのメトリクスは **k=10** で評価しています。Elasticsearch の [Ranking Evaluation API](https://www.elastic.co/docs/reference/elasticsearch/rest-apis/search-rank-eval) を使用して算出しています。

#### Recall@10
上位 10 件に含まれる関連ドキュメントの割合 (網羅性)。

$$\text{Recall@10} = \frac{\text{上位10件中の関連ドキュメント数}}{\text{全関連ドキュメント数}}$$

#### Precision@10
上位 10 件のうち関連ドキュメントである割合 (精度)。

$$\text{Precision@10} = \frac{\text{上位10件中の関連ドキュメント数}}{10}$$

#### nDCG@10 (Normalized Discounted Cumulative Gain)
ランキングの順位と関連度を考慮した評価指標。上位に高関連のドキュメントが来るほど高スコアとなります。

$$\text{DCG@10} = \sum_{i=1}^{10} \frac{rel_i}{\log_2(i+1)}$$

$$\text{nDCG@10} = \frac{\text{DCG@10}}{\text{Ideal DCG@10}}$$

