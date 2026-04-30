# テキスト埋め込みモデル 日本語性能ベンチマーク

## データセット: 尼崎市 Q&A データセット

京都大学が公開している BERT-Based FAQ Retrieval 用データセットを使用しています。

- [BERT-Based FAQ Retrieval (京都大学)](https://nlp.ist.i.kyoto-u.ac.jp/EN/index.php?BERT-Based_FAQ_Retrieval)
- [GitHub リポジトリ](https://github.com/ku-nlp/bert-based-faqir)

| 項目 | 内容 |
|------|------|
| コーパス | 尼崎市の Q&A ドキュメント 1,785 件 |
| クエリ | 検索クエリ 748 件 |
| 適合性判定 (qrels) | クエリとドキュメントのペアに対する関連度スコア (1: やや関連, 2: 高関連) |

## ベンチマークの結果

### Recall@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.823 |
| 2 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.821 |
| 3 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.814 |
| 4 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.806 |
| 5 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.802 |
| 6 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.802 |
| 7 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.792 |
| 8 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.780 |
| 9 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.778 |
| 10 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.773 |
| 11 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.765 |
| 12 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.765 |
| 13 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.762 |
| 14 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.761 |
| 15 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.756 |
| 16 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.753 |
| 17 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.748 |
| 18 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.745 |
| 19 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.740 |
| 20 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.738 |
| 21 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.735 |
| 22 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.734 |
| 23 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.723 |
| 24 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.719 |
| 25 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.715 |
| 26 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.710 |
| 27 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.706 |
| 28 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.698 |
| 29 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.683 |
| 30 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.682 |
| 31 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.673 |
| 32 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.664 |
| 33 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.660 |
| 34 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.645 |
| 35 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.642 |
| 36 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.615 |
| 37 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.600 |
| 38 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.566 |
| 39 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.528 |
| 40 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.511 |
| 41 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.462 |
| 42 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.247 |
| 43 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.199 |
| 44 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.180 |
| 45 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.133 |
| 46 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.130 |

### Precision@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.188 |
| 2 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.187 |
| 3 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.185 |
| 4 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.185 |
| 5 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.183 |
| 6 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.182 |
| 7 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.181 |
| 8 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.178 |
| 9 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.177 |
| 10 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.177 |
| 11 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.177 |
| 12 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.174 |
| 13 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.174 |
| 14 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.174 |
| 15 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.173 |
| 16 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.172 |
| 17 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.172 |
| 18 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.172 |
| 19 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.171 |
| 20 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.170 |
| 21 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.170 |
| 22 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.168 |
| 23 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.167 |
| 24 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.163 |
| 25 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.163 |
| 26 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.163 |
| 27 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.162 |
| 28 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.159 |
| 29 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.158 |
| 30 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.158 |
| 31 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.153 |
| 32 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.152 |
| 33 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.151 |
| 34 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.148 |
| 35 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.148 |
| 36 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.142 |
| 37 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.137 |
| 38 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.123 |
| 39 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.121 |
| 40 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.119 |
| 41 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.108 |
| 42 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.056 |
| 43 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.042 |
| 44 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.038 |
| 45 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.032 |
| 46 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.021 |

### nDCG@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.725 |
| 2 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.708 |
| 3 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.707 |
| 4 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.696 |
| 5 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.691 |
| 6 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.681 |
| 7 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.666 |
| 8 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.666 |
| 9 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.663 |
| 10 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.659 |
| 11 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.652 |
| 12 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.649 |
| 13 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.642 |
| 14 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.637 |
| 15 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.637 |
| 16 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.633 |
| 17 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.628 |
| 18 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.625 |
| 19 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.621 |
| 20 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.620 |
| 21 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.618 |
| 22 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.612 |
| 23 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.600 |
| 24 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.597 |
| 25 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.590 |
| 26 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.590 |
| 27 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.589 |
| 28 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.587 |
| 29 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.586 |
| 30 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.571 |
| 31 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.563 |
| 32 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.556 |
| 33 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.555 |
| 34 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.522 |
| 35 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.521 |
| 36 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.495 |
| 37 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.494 |
| 38 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.486 |
| 39 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.411 |
| 40 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.407 |
| 41 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.356 |
| 42 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.188 |
| 43 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.170 |
| 44 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.127 |
| 45 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.111 |
| 46 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.088 |

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

