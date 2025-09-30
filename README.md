PubMed RAG Medical QA App

This project is a Retrieval-Augmented Generation (RAG) based Medical Question Answering (QA) application.
It fetches abstracts from PubMed, builds embeddings with a biomedical language model, stores them in a FAISS index, and answers medical questions using a hybrid of retrieval + generative QA.

📂 Project Structure

01_fetch_pubmed_abstracts.ipynb → Fetch abstracts from PubMed based on medical keywords.

02_embeddings.ipynb → Generate embeddings for abstracts using BioBERT.

03_build_embeddings_faiss.ipynb → Build FAISS index for similarity search.

04_query_faiss.ipynb → Test search queries and verify retrieved documents.

05_model_integration.ipynb → Integrate QA models (PubMedBERT extractive QA / Flan-T5 hybrid QA).

Other supporting files:

requirements.txt → Python dependencies.

.gitignore → Excluded files (cache, model downloads, large data).

🚀 Features

PubMed Abstract Retrieval → Automatically fetch research abstracts.

Biomedical Embeddings → Uses BioBERT for domain-specific embeddings.

Efficient Search → FAISS for fast similarity search over thousands of documents.

QA Models →

Extractive QA with PubMedBERT.

Hybrid QA (retrieval + Flan-T5 summarization) for readable answers.

⚙️ Installation

Clone this repo and install dependencies:

git clone https://github.com/your-username/PubMed-RAG-Medical-QA-App.git
cd PubMed-RAG-Medical-QA-App
pip install -r requirements.txt

▶️ Usage

Run 01_fetch_pubmed_abstracts.ipynb to download abstracts.

Run 02_embeddings.ipynb to create embeddings.

Run 03_build_embeddings_faiss.ipynb to build FAISS index.

Run 04_query_faiss.ipynb to test retrieval.

Run 05_model_integration.ipynb to ask medical questions via QA models.

📊 Example Questions

What are the symptoms of diabetes?

What is aspirin used for?

How does gut microbiota affect drug absorption?

Adverse effects of metformin?

⚠️ Disclaimer

This app is for educational and research purposes only.
It is not a substitute for professional medical advice

