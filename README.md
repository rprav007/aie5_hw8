# aie5_hw8

Question #1 - What is the purpose of the `chunk_overlap` parameter in the `RecursiveCharacterTextSplitter`?

The chunk_overlap parameter in the RecursiveCharacterTextSplitter serves a crucial purpose, which is to maintain context and prevent information loss when splitting text into chunks. Chunk overlap helps with the following
* Contextual Continuity
* Preventing Information Loss
* Improved Retrieval Accuracy

Hence its a very important parameter while tuning RAG applications. It guards against arbitrary chunking and provides enough context for the LLM to provide accurate responses

Question #2 - Which system performed better, on what metrics, and why?
