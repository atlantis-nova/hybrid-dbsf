# Please cite
Algorithm: **distribution-based score fusion (also called DBSF, [hybrid-dbsf](https://arxiv.org/html/2410.20878v1), [distribution-based rank fusion](https://github.com/deepset-ai/haystack/issues/7914))**<br>
Author: **Michelangiolo Mazzeschi** - [original source](https://medium.com/plain-simple-software/distribution-based-score-fusion-dbsf-a-new-approach-to-vector-search-ranking-f87c37488b18)<br>
Published: **2nd November 2023**

***Note: According to this [arxiv paper](https://arxiv.org/html/2410.20878v1), hybrid-dbsf is now **the top semantic search algorithm in the world**<br>

# hybrid-dbsf
Note: This formula was created as the first multimodal algorithm capable of combining **images and text** in the same search. However, it has been shown how it beats all existing benchmarks even in regular vector search, making it the #1 search algorithm (with new applications in RAG).
<br><br>
![image](https://github.com/user-attachments/assets/36e12dba-670f-4e94-a031-8d586b4c02f3)

### Limitations and Improvements
The current implementation uses a sigma value of 3 as a replacement for minmax. This implementation, however, is based on the assumption that the cosine similarity score distribution is normal, which is never the case.<br>
To obtain even better results, quantiles (respectively [99, 1] for the tail extremes of the distribution, should be used.

# citations

- llama-index [(link)](https://docs.llamaindex.ai/en/stable/examples/retrievers/relative_score_dist_fusion/)
- Epsilla [(link)](https://epsilla-inc.gitbook.io/epsilladb/epsilla-vector-database/advanced-topics/hybrid-search)
- Qdrant [(link)](https://qdrant.tech/documentation/concepts/hybrid-queries/)
- Weaviate [(link)](https://haystack.deepset.ai/release-notes/2.3.0)
- Julep-ai [(link)](https://github.com/julep-ai/julep/blob/704fdf9b3035263800408ac46b9708a973d26b59/agents-api/agents_api/models/docs/search_docs_hybrid.py#L15)
- Haystack [(link)](https://github.com/deepset-ai/haystack/issues/7914)
- Upstash [(link)](https://upstash.com/docs/vector/features/hybridindexes)
- Redis [(link)](https://github.com/redis-developer/hybrid-js)
- AutoRAG: Automated Framework for optimization of Retrieval Augmented Generation Pipeline [(link)](https://arxiv.org/html/2410.20878v1)

  ![image](https://github.com/user-attachments/assets/816af563-e139-40f4-9f80-565f41fccb47)<br>
  In the paper it is depicted as the #1 known algorithm for retrieval

# license
As for all my algorithms, I have chosen the license that (to the extent of my knowledge) should allow for the most open usage and personalization of this algorithm.<br>
If that is not the case, please open an issue outlining the license limitations and I will do my best to apply the necessary changes to resolve them, as long as they align with the primary objectives of code democratization. 
