# RAG-based Medical Chatbot

A complete medical chatbot built using LLMs, LangChain, Pinecone, Flask, and AWS. This project demonstrates Retrieval-Augmented Generation (RAG) for answering medical queries using a custom knowledge base.

## Features
- Chatbot interface for medical Q&A
- Uses LLMs and LangChain for natural language understanding
- Pinecone for vector search and retrieval
- Flask backend for API and web server
- AWS integration for scalable deployment

## Project Structure
```
app.py                # Main Flask application
requirements.txt      # Python dependencies
Dockerfile            # Containerization
src/                  # Source code (helpers, prompts)
data/                 # Medical knowledge base (PDF)
research/             # Notebooks for experiments
static/, templates/   # Frontend assets
```

## Setup
1. **Clone the repository:**
   ```powershell
   git clone https://github.com/tusharchothe/RAG-based-chatbot.git
   cd RAG-based-chatbot
   ```
2. **Install dependencies:**
   ```powershell
   pip install -r requirements.txt
   ```
3. **Run the application:**
   ```powershell
   python app.py
   ```
4. **Access the chatbot:**
   Open your browser at `http://localhost:5000`

## Docker
To run with Docker:
```powershell
   docker build -t rag-medical-chatbot .
   docker run -p 5000:5000 rag-medical-chatbot
```

## Deployment
- You can deploy on AWS using Elastic Beanstalk, ECS, or Lambda (with container support).
- For cloud deployment, set environment variables for API keys and secrets as needed.

## Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License.
