# Semantic_Hunt
A semantic search engine is an advanced type of search engine that understands the meaning and context behind words, rather than just matching exact keywords in a document. Unlike traditional search engines, which rely on keyword-based searches, a semantic search engine focuses on the intent behind the user's query and tries to deliver more relevant and accurate results.
Here’s how it works:

Text Extraction:

The search engine first extracts all the text from PDF files using a tool called PyMuPDF. This makes the content of the PDFs searchable.
Understanding the Meaning (Embedding):

Instead of looking for keywords, your search engine uses a model called BERT (a type of AI language model) to convert the text into numbers (called embeddings) that represent the meaning of the text. It does the same for the user's query, which allows it to compare the meaning, not just the words.
Efficient Search (Indexing):

To make the search fast, you used a tool called FAISS to organize and index all the document embeddings. This allows the system to quickly find the most relevant parts of the documents that match the query’s meaning.
User Interface:

The front-end of your search engine, built with Streamlit, is simple and interactive. Users type their search query, and the most relevant answer pops up right away. If they want more answers, they can click on a button to see other relevant responses.
Page-Level Search:

To make the system faster and more efficient, your search engine looks for answers at the page level (instead of searching through every paragraph). This helps users find the right information more quickly.
