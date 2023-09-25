# Legal Chatbot
## Problem Statement

1. **Issue**: Inefficiencies and complexities linked with manual legal document creation.
    - **Example**: In a contract, when Company A and Company B agree on purchasing 'green widgets,' Company B is tasked with delivering 'high-quality' ones, but the term 'high-quality' remains undefined.

2. **Issue**: Utilizing a legal chatbot powered by technology to offer precise responses to inquiries concerning legal cases and laws.

___
## Idea Description

1. **Automated Legal Document Generation**
   
   Generate legal documents through customizable templates, incorporating user-provided information. Utilize Natural Language Processing (NLP) algorithms to extract crucial details from user inputs.

2. **Legal Chatbot for Precise Answers**

   Develop a legal chatbot employing advanced technology to deliver accurate responses to inquiries concerning legal cases and laws.
___

## Quickstart
- To start parsing user queries into the application, launch the terminal from the project directory and run the following command:
`poetry run python main.py "<user query>"`
- For example, `poetry run python main.py "Can I use heater and iron in the hostel?"`
- Note: Omit the prepended `poetry run` if you are NOT using Poetry
___
## Tools
- **LangChain**: Framework for developing applications powered by language models
- **C Transformers**: Python bindings for the Transformer models implemented in C/C++ using GGML library
- **FAISS**: Open-source library for efficient similarity search and clustering of dense vectors.
- **Sentence-Transformers (all-MiniLM-L6-v2)**: Open-source pre-trained transformer model for embedding text to a 384-dimensional dense vector space for tasks like clustering or semantic search.
- **Llama-2-7B-Chat**: Open-source fine-tuned Llama 2 model designed for chat dialogue. Leverages publicly available instruction datasets and over 1 million human annotations. 
- **Poetry**: Tool for dependency management and Python packaging

___
## Files and Content
- `/assets`: Images relevant to the project
- `/config`: Configuration files for LLM application
- `/data`: Dataset used for this project (i.e., Manchester United FC 2022 Annual Report - 177-page PDF document)
- `/models`: Binary file of GGML quantized LLM model (i.e., Llama-2-7B-Chat) 
- `/src`: Python codes of key components of LLM application, namely `llm.py`, `utils.py`, and `prompts.py`
- `/vectorstore`: FAISS vector store for documents
- `db_build.py`: Python script to ingest dataset and generate FAISS vector store
- `main.py`: Main Python script to launch the application and to pass user query via command line
- `pyproject.toml`: TOML file to specify which versions of the dependencies used (Poetry)
- `requirements.txt`: List of Python dependencies (and version)
___
