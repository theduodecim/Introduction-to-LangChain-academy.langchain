# Setup con OpenRouter (free)

## Keys necesarias

| Key | Dónde conseguirla | Costo |
|-----|-------------------|-------|
| `OPENAI_API_KEY` | [openrouter.ai/keys](https://openrouter.ai/keys) | Gratis |
| `TAVILY_API_KEY` | [tavily.com](https://tavily.com) | Gratis (1000/mes) |
| `LANGSMITH_API_KEY` | [smith.langchain.com](https://smith.langchain.com) | Gratis |

## Modelo usado
`nvidia/nemotron-3-ultra-550b-a55b:free` — el más potente del free tier de OpenRouter.

## Setup en Codespaces

```bash
# 1. Instalar uv
pip install uv

# 2. Instalar dependencias
uv sync

# 3. Correr notebooks
uv run jupyter lab
```

## Notas

- **1.4_multimodal_messages.ipynb** — La celda de audio no va a funcionar con modelos free (requiere gpt-4o-audio). El resto del notebook sí funciona.
- **bonus_rag.ipynb** — Usa `OpenAIEmbeddings` para embeddings. Si querés usarlo necesitás una key de OpenAI para esa parte, o podés saltear el bonus.
- Todos los demás notebooks funcionan 100% con OpenRouter free.
