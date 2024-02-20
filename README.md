# RAG Sample Data

A few sample data files, to be used for demonstrating RAG search with MongoDB.

This repository is designed to be used by LangChain's [GitHub document loader](https://python.langchain.com/docs/integrations/document_loaders/github#load-github-file-content).
```python
loader = GithubFileLoader(
    repo="mongodb-developer/rag-app-sample-data",
    access_token=ACCESS_TOKEN,
    github_api_url="https://api.github.com",
    file_filter=lambda file_path: file_path.endswith(
        ".txt"
    ),  # load all text files.
)
```