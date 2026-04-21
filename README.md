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



streamlit run app_multiple.py --server.port 8080