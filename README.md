# Abstract
Technology has opened up a new era of mental health care and information gathering, providing new means to access aid, connect to a peer counselor, and track progress. Chezlong is an Arabic text-based chatbot powered by the most modern NLP techniques. It aims to give guidance to those who need quick mental support. The development cycle is based on using the GPT-3.5 Large Language Model for Retrieval Augmented Generation (RAG). RAG is used on Arabic psychological articles, originally scraped from the nafsy.net website. Cleaning, preprocessing, and topic modeling have been applied to prepare and explore the dataset. The chunked dataset is stored as vectors in Pinecone. Similarity search is done to retrieve query-related source knowledge from the dataset to answer a user query.

# Key Points
- Cleaned and preprocessed Arabic psychological texts scraped from nafsy.net using NLTK and HuggingFace.
- Applied BERTopic modeling to explore topic distributions and deduplicate the data.
- Synthesized a QA dataset from the original corpus using GPT to support potential fine-tuning.
- Stored chunked text embeddings in Pinecone to enable scalable and efficient semantic search.
- Implemented similarity search to retrieve contextually relevant passages for user queries.
- Prompt-engineered the engine's query to integrate GPT-3.5 with Retrieval Augmented Generation (RAG),
ensuring domain-relevant answers.
- Connected all previous components within a LangChain pipeline for end-to-end user query handling.
- Experimented with multiple LLMs and semantic embedding models to optimize performance for Arabic.
