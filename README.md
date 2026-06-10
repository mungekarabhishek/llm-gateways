# LLM Gateways

A Python project demonstrating unified access to multiple Large Language Model (LLM) providers through LiteLLM, featuring automatic fallbacks, cost tracking, and response caching.

## 🚀 Features

- **Multi-Provider Support**: Seamlessly integrate with OpenAI, Groq, Google Gemini, and other LLM providers
- **Automatic Fallbacks**: Built-in failover mechanism when primary LLM provider is unavailable
- **Cost Tracking**: Monitor token usage and calculate costs for each API call
- **Response Caching**: Reduce costs and improve response times with intelligent caching
- **Unified Interface**: Single API for multiple LLM providers using LiteLLM

## 📋 Prerequisites

- Python >= 3.12
- API keys for the LLM providers you want to use:
  - OpenAI API Key
  - Groq API Key
  - Google API Key

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.ibm.com/amungeka/llm-gateways.git
cd llm-gateways
```

2. Install dependencies using uv (recommended) or pip:
```bash
# Using uv
uv sync

3. Create a `.env` file in the project root and add your API keys:
```env
OPENAI_API_KEY=your_openai_api_key_here
GROQ_API_KEY=your_groq_api_key_here
GOOGLE_API_KEY=your_google_api_key_here
```

## 📦 Dependencies

- **litellm**: Unified interface for multiple LLM providers
- **langchain**: Framework for building LLM applications
- **langchain-community**: Community integrations for LangChain
- **langchain-litellm**: LiteLLM integration for LangChain
- **langchain-openai**: OpenAI integration for LangChain
- **google-genai**: Google Generative AI SDK
- **python-dotenv**: Environment variable management
- **kernel**: Additional utilities


## 📓 Jupyter Notebook

The project includes a comprehensive Jupyter notebook (`llm-gateways.ipynb`) with interactive examples demonstrating:

- Basic LLM completions across multiple providers
- Error handling and provider comparison
- Automatic fallback mechanisms
- Cost tracking and token usage analysis
- Response caching for performance optimization

To run the notebook:
```bash
jupyter notebook llm-gateways.ipynb
```

## 🏗️ Project Structure

```
llm-gateways/
├── main.py                 # Main application entry point
├── llm-gateways.ipynb     # Interactive examples and demonstrations
├── pyproject.toml         # Project dependencies and metadata
├── uv.lock                # Dependency lock file
├── .env                   # Environment variables (create this)
├── .gitignore            # Git ignore rules
└── README.md             # This file
```

## 🔧 Configuration

### Supported Models

**OpenAI:**
- `gpt-4o-mini`
- `gpt-4`
- `gpt-3.5-turbo`

**Groq:**
- `groq/llama-3.3-70b-versatile`
- `groq/mixtral-8x7b-32768`

**Google:**
- `gemini-1.5-flash`
- `gemini-2.5-flash-lite`
- `gemini-pro`

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
