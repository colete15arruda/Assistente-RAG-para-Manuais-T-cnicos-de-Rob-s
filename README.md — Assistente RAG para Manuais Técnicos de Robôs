# 🚀 Assistente RAG para Manuais Técnicos de Robôs

[![Python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)]

## 📖 Descrição
O Assistente RAG para Manuais Técnicos de Robôs é uma aplicação de IA baseada em Retrieval-Augmented Generation (RAG) que permite consultar manuais técnicos e documentação de robótica, incluindo:

- PDFs de datasheets de sensores e motores  
- Guias de Arduino e ESP32  
- Documentação ROS2  

O sistema processa os documentos, gera embeddings, armazena em um vector database e utiliza um LLM para fornecer respostas contextuais precisas, reduzindo erros de interpretação.

---

## 🎯 Objetivos
- Tornar a consulta de manuais técnicos rápida e eficiente  
- Reduzir erros de interpretação da documentação  
- Demonstrar integração prática entre LLMs, embeddings e vector databases  

---

## 🛠️ Tecnologias e Bibliotecas
- Python 3.10+  
- LangChain – pipeline RAG  
- OpenAI ou Azure OpenAI – LLM e embeddings  
- ChromaDB ou FAISS – vector database  
- PyMuPDF ou pdfplumber – extração de texto de PDFs  
- FastAPI – API para perguntas  
- uvicorn – servidor ASGI  

---

## 📂 Estrutura do Projeto

argorag/
├── data/
│ ├── raw_pdfs/ # PDFs originais
│ └── chunks/ # Textos processados em pedaços
├── src/
│ ├── ingest_docs.py # leitura e chunking de PDFs
│ ├── embeddings.py # gera embeddings e armazena no vector DB
│ ├── retriever.py # recupera trechos relevantes
│ ├── rag_pipeline.py # pipeline de RAG
│ └── api.py # FastAPI para interface de perguntas
├── requirements.txt
└── README.md


---

## ⚡ Como Rodar

### 1. Clonar o repositório
```bash
git clone https://github.com/colete15arruda/Assistente-RAG-para-Manuais-Tecnicos-de-Robos.git
cd argorag
2. Criar e ativar ambiente virtual
python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux / Mac
source .venv/bin/activate
3. Instalar dependências
pip install -r requirements.txt
4. Configurar chave da OpenAI
Crie um arquivo .env na raiz do projeto:

OPENAI_API_KEY=SUA_CHAVE_AQUI
5. Processar PDFs e gerar embeddings
python src/ingest_docs.py
python src/embeddings.py
6. Rodar API
uvicorn src.api:app --reload
7. Testar perguntas
"Qual a tensão recomendada para o motor X?"
"Como ligar o sensor ultrassônico HC-SR04?"
"Como configurar tópicos no ROS2?"
✅ Resultado
O assistente retorna respostas contextuais baseadas nos PDFs processados, com referência ao trecho original, tornando a consulta técnica rápida, confiável e organizada.

📌 Licença
Este projeto está licenciado sob a MIT License. Veja o arquivo LICENSE para mais detalhes.

👩‍💻 Autor
Gabrielle Arruda — Portfólio de IA aplicada à robótica e automação.
