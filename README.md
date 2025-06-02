# Multi-Agent-Localized-Weather-Information
 Multi-Agent RAG System for Localized Weather Information

This project demonstrates a multi-agent Retrieval-Augmented Generation (RAG) system designed to fetch and translate weather information for specific locations. It leverages `smolagents` for agent orchestration, `LiteLLM` for model interaction, and `Helsinki-NLP/opus-mt` for machine translation.

## Features

* **Intelligent Location Extraction**: Attempts to identify cities from natural language queries.
* **Country and Language Detection**: Determines the country associated with a city and identifies the appropriate target language for translation.
* **Dynamic Weather Retrieval**: Uses a `retriever_agent` to search for weather information.
* **Multi-lingual Output**: Translates weather information into the local language of the detected country if it's not English.
* **Modular Agent Design**: Utilizes `smolagents` for clear separation of concerns (retrieval, search).

 **Clone the repository** (once uploaded to GitHub):
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name

    ```

## Usage

Run the `multi_rag.py` script and call the `manager_agent` function with your query.

```python
# Example usage from multi_rag.py
print(manager_agent("Berlin weather today"))
print(manager_agent("Paris weather today"))
print(manager_agent("Italy weather today"))
