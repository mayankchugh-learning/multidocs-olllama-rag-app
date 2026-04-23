# multidocs-olllama-rag-app

# Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Pull required models
ollama pull llama3.2           # LLM for answer generation (~2 GB)
ollama pull nomic-embed-text   # Embedding model (~274 MB)

# Start Ollama server
ollama serve &

# Verify models are running
curl http://localhost:11434/api/tags



uv pip install -r multidocs-olllama-rag-app/requirements.txt

streamlit run multidocs-olllama-rag-app/app_multiple.py --server.port 8080

source .venv/bin/activate


streamlit run app.py --server.address=0.0.0.0 --server.port=8501

streamlit run multidocs-olllama-rag-app/app_multiple.py  --server.address=0.0.0.0 --server.port=8501

streamlit run app_multiple.py  --server.address=0.0.0.0 --server.port=8501

sudo apt-get install  lsof

lsof -i :8501
kill -9 [pid]