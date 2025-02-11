# aie5_hw8

Question #1 - What is the purpose of the `chunk_overlap` parameter in the `RecursiveCharacterTextSplitter`?

The chunk_overlap parameter in the RecursiveCharacterTextSplitter serves a crucial purpose, which is to maintain context and prevent information loss when splitting text into chunks. Chunk overlap helps with the following
* Contextual Continuity
* Preventing Information Loss
* Improved Retrieval Accuracy

Hence its a very important parameter while tuning RAG applications. It guards against arbitrary chunking and provides enough context for the LLM to provide accurate responses

Question #2 - Which system performed better, on what metrics, and why?

Before using Cohere re-ranking we got the following metrics

{'context_recall': 0.8708, 'faithfulness': nan, 'factual_correctness': 0.4791, 'answer_relevancy': 0.9524, 'context_entity_recall': 0.4238, 'noise_sensitivity_relevant': 0.3964}

After using Cohere re-ranking we got the following metrics

{'context_recall': 0.8333, 'faithfulness': 0.5714, 'factual_correctness': 0.5255, 'answer_relevancy': 0.9510, 'context_entity_recall': 0.4409, 'noise_sensitivity_relevant': 0.2436}

Looking at the 2 results the system performed better after using the re-ranking model from Cohere. There was remarkable difference in factual correctness (better) and less noise (filtered irrelevant information). The possible reasons are as follows:

* Semantic Relevance Refinement
      * Beyond Keyword Matching
      * Contextual Understanding
      * Intent Alignment
* Improved Precision
      * Filtering irrelevant results
      * Focus on top results
* Enhanced Contextual Coherence
* Model Training and Capabilities
      * Better algorithm
