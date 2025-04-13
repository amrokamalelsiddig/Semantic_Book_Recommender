# Semantic_Book_Recommender

an intelligent book recommendation system powered by large language models and semantic search. this project transforms book descriptions into mathematical embeddings to enable precise, content-based recommendations — helping readers discover their next favorite book without relying on traditional ratings or categories

## 🔧 Technologies Used

- [`transformers`](https://github.com/huggingface/transformers) by Hugging Face  
- `facebook/bart-large-mnli` for zero-shot classification  
- `torch` (CPU-based inference)  
- `langchain` + `chromadb` for vector search and storage  
- `pandas`, `seaborn`, `matplotlib` for EDA  
- `gradio` (planned) for UI


---

## 📦 Data Source

- **7K Books Dataset from Kaggle**  
  Contains: title, subtitle, author, category, description, ISBN, cover image URL, ratings, and more.

---

## 🛠 Features Implemented

- ✅ EDA: Missing value visualization, correlation heatmaps  
- ✅ Filtering: Removing short or incomplete descriptions  
- ✅ Feature Engineering: Combining title + subtitle, tagging descriptions  
- ✅ Zero-Shot Classification: Label books as “Fiction” or “Nonfiction”  
- ✅ Semantic Preparation: Data structured for vector database loading

---


---

## 🧪 Try It Locally

```bash
git clone https://github.com/amrokamalelsiddig/Semantic_Book_Recommender.git
cd Semantic_Book_Recommender


create .env file and place your api keys for openai and hugging face 
python -m venv book
source book/bin/activate

pip install -r requirements.txt

python3 gradio-dashboard.py

then visit http://127.0.0.1:7860/